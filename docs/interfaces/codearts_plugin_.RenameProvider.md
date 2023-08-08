[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / RenameProvider

# Interface: RenameProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).RenameProvider

The rename provider interface defines the contract between extensions and
the [rename](https://code.visualstudio.com/docs/editor/editingevolved#_rename-symbol)-feature.

## Table of contents

### Methods

- [prepareRename](codearts_plugin_.RenameProvider.md#preparerename)
- [provideRenameEdits](codearts_plugin_.RenameProvider.md#providerenameedits)

## Methods

### prepareRename

▸ `Optional` **prepareRename**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Range`](../classes/codearts_plugin_.Range.md) \| { `placeholder`: `string` ; `range`: [`Range`](../classes/codearts_plugin_.Range.md)  }\>

Optional function for resolving and validating a position *before* running rename. The result can
be a range or a range and a placeholder text. The placeholder text should be the identifier of the symbol
which is being renamed - when omitted the text in the returned range is used.

*Note:* This function should throw an error or return a rejected thenable when the provided location
doesn't allow for a rename.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which rename will be invoked. |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | The position at which rename will be invoked. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Range`](../classes/codearts_plugin_.Range.md) \| { `placeholder`: `string` ; `range`: [`Range`](../classes/codearts_plugin_.Range.md)  }\>

The range or range and placeholder text of the identifier that is to be renamed. The lack of a result can signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:3714](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3714)

___

### provideRenameEdits

▸ **provideRenameEdits**(`document`, `position`, `newName`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`WorkspaceEdit`](../classes/codearts_plugin_.WorkspaceEdit.md)\>

Provide an edit that describes changes that have to be made to one
or many resources to rename a symbol to a different name.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | The position at which the command was invoked. |
| `newName` | `string` | The new name of the symbol. If the given name is not valid, the provider must return a rejected promise. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`WorkspaceEdit`](../classes/codearts_plugin_.WorkspaceEdit.md)\>

A workspace edit or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:3699](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3699)
