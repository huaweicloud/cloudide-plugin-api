**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CodeLensProvider

# Interface: CodeLensProvider

A code lens provider adds [commands](#Command) to source text. The commands will be shown
as dedicated horizontal lines in between the source text.

## Hierarchy

* **CodeLensProvider**

## Index

### Properties

* [onDidChangeCodeLenses](_index_d_._plugin_.codelensprovider.md#ondidchangecodelenses)

### Methods

* [provideCodeLenses](_index_d_._plugin_.codelensprovider.md#providecodelenses)
* [resolveCodeLens](_index_d_._plugin_.codelensprovider.md#resolvecodelens)

## Properties

### onDidChangeCodeLenses

• `Optional` **onDidChangeCodeLenses**: [Event](_index_d_._plugin_.event.md)\<void>

*Defined in [index.d.ts:2286](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2286)*

An optional event to signal that the code lenses from this provider have changed.

## Methods

### provideCodeLenses

▸ **provideCodeLenses**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[CodeLens](../classes/_index_d_._plugin_.codelens.md)[]>

*Defined in [index.d.ts:2298](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2298)*

Compute a list of [lenses](#CodeLens). This call should return as fast as possible and if
computing the commands is expensive implementors should only return code lens objects with the
range set and implement [resolve](#CodeLensProvider.resolveCodeLens).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[CodeLens](../classes/_index_d_._plugin_.codelens.md)[]>

An array of code lenses or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

___

### resolveCodeLens

▸ `Optional`**resolveCodeLens**(`codeLens`: [CodeLens](../classes/_index_d_._plugin_.codelens.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[CodeLens](../classes/_index_d_._plugin_.codelens.md)>

*Defined in [index.d.ts:2308](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2308)*

This function will be called for each visible code lens, usually when scrolling and after
calls to [compute](#CodeLensProvider.provideCodeLenses)-lenses.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`codeLens` | [CodeLens](../classes/_index_d_._plugin_.codelens.md) | code lens that must be resolved. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[CodeLens](../classes/_index_d_._plugin_.codelens.md)>

The given, resolved code lens or thenable that resolves to such.
