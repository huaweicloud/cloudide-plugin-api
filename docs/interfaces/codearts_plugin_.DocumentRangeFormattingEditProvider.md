[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentRangeFormattingEditProvider

# Interface: DocumentRangeFormattingEditProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentRangeFormattingEditProvider

The document formatting provider interface defines the contract between extensions and
the formatting-feature.

## Table of contents

### Methods

- [provideDocumentRangeFormattingEdits](codearts_plugin_.DocumentRangeFormattingEditProvider.md#providedocumentrangeformattingedits)

## Methods

### provideDocumentRangeFormattingEdits

▸ **provideDocumentRangeFormattingEdits**(`document`, `range`, `options`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TextEdit`](../classes/codearts_plugin_.TextEdit.md)[]\>

Provide formatting edits for a range in a document.

The given range is a hint and providers can decide to format a smaller
or larger range. Often this is done by adjusting the start and end
of the range to full syntax nodes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `range` | [`Range`](../classes/codearts_plugin_.Range.md) | The range which should be formatted. |
| `options` | [`FormattingOptions`](codearts_plugin_.FormattingOptions.md) | Options controlling formatting. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TextEdit`](../classes/codearts_plugin_.TextEdit.md)[]\>

A set of text edits or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:3965](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L3965)
