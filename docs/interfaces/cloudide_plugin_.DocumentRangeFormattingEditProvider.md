[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DocumentRangeFormattingEditProvider

# Interface: DocumentRangeFormattingEditProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DocumentRangeFormattingEditProvider

The document formatting provider interface defines the contract between extensions and
the formatting-feature.

## Table of contents

### Methods

- [provideDocumentRangeFormattingEdits](cloudide_plugin_.DocumentRangeFormattingEditProvider.md#providedocumentrangeformattingedits)

## Methods

### provideDocumentRangeFormattingEdits

▸ **provideDocumentRangeFormattingEdits**(`document`, `range`, `options`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`undefined` \| [`TextEdit`](../classes/cloudide_plugin_.TextEdit.md)[]\>

Provide formatting edits for a range in a document.

The given range is a hint and providers can decide to format a smaller
or larger range. Often this is done by adjusting the start and end
of the range to full syntax nodes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `range` | [`Range`](../classes/cloudide_plugin_.Range.md) | The range which should be formatted. |
| `options` | [`FormattingOptions`](cloudide_plugin_.FormattingOptions.md) | Options controlling formatting. |
| `token` | `undefined` \| [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`undefined` \| [`TextEdit`](../classes/cloudide_plugin_.TextEdit.md)[]\>

A set of text edits or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:8381](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8381)
