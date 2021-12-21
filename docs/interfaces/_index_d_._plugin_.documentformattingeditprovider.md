**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DocumentFormattingEditProvider

# Interface: DocumentFormattingEditProvider

The document formatting provider interface defines the contract between extensions and
the formatting-feature.

## Hierarchy

* **DocumentFormattingEditProvider**

## Index

### Methods

* [provideDocumentFormattingEdits](_index_d_._plugin_.documentformattingeditprovider.md#providedocumentformattingedits)

## Methods

### provideDocumentFormattingEdits

▸ **provideDocumentFormattingEdits**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `options`: [FormattingOptions](_index_d_._plugin_.formattingoptions.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[TextEdit](../classes/_index_d_._plugin_.textedit.md)[]>

*Defined in [index.d.ts:3673](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3673)*

Provide formatting edits for a whole document.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`options` | [FormattingOptions](_index_d_._plugin_.formattingoptions.md) | Options controlling formatting. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[TextEdit](../classes/_index_d_._plugin_.textedit.md)[]>

A set of text edits or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.
