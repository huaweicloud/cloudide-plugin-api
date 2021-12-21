**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CodeLensProvider

# Interface: CodeLensProvider\<T>

A code lens provider adds [commands](#Command) to source text. The commands will be shown
as dedicated horizontal lines in between the source text.

## Type parameters

Name | Type | Default |
------ | ------ | ------ |
`T` | [CodeLens](../classes/_index_d_._plugin_.codelens.md) | CodeLens |

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

*Defined in [index.d.ts:2508](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2508)*

An optional event to signal that the code lenses from this provider have changed.

## Methods

### provideCodeLenses

▸ **provideCodeLenses**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T[]>

*Defined in [index.d.ts:2520](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2520)*

Compute a list of [lenses](#CodeLens). This call should return as fast as possible and if
computing the commands is expensive implementors should only return code lens objects with the
range set and implement [resolve](#CodeLensProvider.resolveCodeLens).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T[]>

An array of code lenses or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

___

### resolveCodeLens

▸ `Optional`**resolveCodeLens**(`codeLens`: T, `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T>

*Defined in [index.d.ts:2530](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2530)*

This function will be called for each visible code lens, usually when scrolling and after
calls to [compute](#CodeLensProvider.provideCodeLenses)-lenses.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`codeLens` | T | Code lens that must be resolved. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T>

The given, resolved code lens or thenable that resolves to such.
