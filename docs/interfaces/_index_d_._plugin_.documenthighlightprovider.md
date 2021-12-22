**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DocumentHighlightProvider

# Interface: DocumentHighlightProvider

The document highlight provider interface defines the contract between extensions and
the word-highlight-feature.

## Hierarchy

* **DocumentHighlightProvider**

## Index

### Methods

* [provideDocumentHighlights](_index_d_._plugin_.documenthighlightprovider.md#providedocumenthighlights)

## Methods

### provideDocumentHighlights

▸ **provideDocumentHighlights**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `position`: [Position](../classes/_index_d_._plugin_.position.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[DocumentHighlight](../classes/_index_d_._plugin_.documenthighlight.md)[]>

*Defined in [index.d.ts:2851](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2851)*

Provide a set of document highlights, like all occurrences of a variable or
all exit-points of a function.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | The position at which the command was invoked. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[DocumentHighlight](../classes/_index_d_._plugin_.documenthighlight.md)[]>

An array of document highlights or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.
