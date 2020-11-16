**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / RenameProvider

# Interface: RenameProvider

The rename provider interface defines the contract between extensions and
the [rename](https://code.visualstudio.com/docs/editor/editingevolved#_rename-symbol)-feature.

## Hierarchy

* **RenameProvider**

## Index

### Methods

* [prepareRename](_index_d_._plugin_.renameprovider.md#preparerename)
* [provideRenameEdits](_index_d_._plugin_.renameprovider.md#providerenameedits)

## Methods

### prepareRename

▸ `Optional`**prepareRename**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `position`: [Position](../classes/_index_d_._plugin_.position.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Range](../classes/_index_d_._plugin_.range.md) \| { placeholder: string ; range: [Range](../classes/_index_d_._plugin_.range.md)  }>

*Defined in [index.d.ts:3180](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3180)*

Optional function for resolving and validating a position *before* running rename. The result can
be a range or a range and a placeholder text. The placeholder text should be the identifier of the symbol
which is being renamed - when omitted the text in the returned range is used.

*Note: * This function should throw an error or return a rejected thenable when the provided location
doesn't allow for a rename.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which rename will be invoked. |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | The position at which rename will be invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Range](../classes/_index_d_._plugin_.range.md) \| { placeholder: string ; range: [Range](../classes/_index_d_._plugin_.range.md)  }>

The range or range and placeholder text of the identifier that is to be renamed. The lack of a result can signaled by returning `undefined` or `null`.

___

### provideRenameEdits

▸ **provideRenameEdits**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `position`: [Position](../classes/_index_d_._plugin_.position.md), `newName`: string, `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[WorkspaceEdit](../classes/_index_d_._plugin_.workspaceedit.md)>

*Defined in [index.d.ts:3165](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3165)*

Provide an edit that describes changes that have to be made to one
or many resources to rename a symbol to a different name.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | The position at which the command was invoked. |
`newName` | string | The new name of the symbol. If the given name is not valid, the provider must return a rejected promise. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[WorkspaceEdit](../classes/_index_d_._plugin_.workspaceedit.md)>

A workspace edit or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.
