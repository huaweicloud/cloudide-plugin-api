**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DocumentRangeFormattingEditProvider

# Interface: DocumentRangeFormattingEditProvider

The document formatting provider interface defines the contract between extensions and
the formatting-feature.

## Hierarchy

* **DocumentRangeFormattingEditProvider**

## Index

### Methods

* [provideDocumentRangeFormattingEdits](_index_d_._plugin_.documentrangeformattingeditprovider.md#providedocumentrangeformattingedits)

## Methods

### provideDocumentRangeFormattingEdits

▸ **provideDocumentRangeFormattingEdits**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `range`: [Range](../classes/_index_d_._plugin_.range.md), `options`: [FormattingOptions](_index_d_._plugin_.formattingoptions.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[TextEdit](../classes/_index_d_._plugin_.textedit.md)[]>

*Defined in [index.d.ts:3696](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3696)*

Provide formatting edits for a range in a document.

The given range is a hint and providers can decide to format a smaller
or larger range. Often this is done by adjusting the start and end
of the range to full syntax nodes.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`range` | [Range](../classes/_index_d_._plugin_.range.md) | The range which should be formatted. |
`options` | [FormattingOptions](_index_d_._plugin_.formattingoptions.md) | Options controlling formatting. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[TextEdit](../classes/_index_d_._plugin_.textedit.md)[]>

A set of text edits or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.
