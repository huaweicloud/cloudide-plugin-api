**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ReferenceProvider

# Interface: ReferenceProvider

The reference provider interface defines the contract between extensions and
the [find references](https://code.visualstudio.com/docs/editor/editingevolved#_peek)-feature.

## Hierarchy

* **ReferenceProvider**

## Index

### Methods

* [provideReferences](_index_d_._plugin_.referenceprovider.md#providereferences)

## Methods

### provideReferences

▸ **provideReferences**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `position`: [Position](../classes/_index_d_._plugin_.position.md), `context`: [ReferenceContext](_index_d_._plugin_.referencecontext.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Location](../classes/_index_d_._plugin_.location.md)[]>

*Defined in [index.d.ts:3099](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3099)*

Provide a set of project-wide references for the given position and document.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | The position at which the command was invoked. |
`context` | [ReferenceContext](_index_d_._plugin_.referencecontext.md) | - |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token.  |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Location](../classes/_index_d_._plugin_.location.md)[]>

An array of locations or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.
