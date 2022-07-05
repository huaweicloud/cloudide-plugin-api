[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentRangeFormattingEditProvider

# Interface: DocumentRangeFormattingEditProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentRangeFormattingEditProvider

## Table of contents

### Methods

- [provideDocumentRangeFormattingEdits](codearts_plugin_.DocumentRangeFormattingEditProvider.md#providedocumentrangeformattingedits)

## Methods

### provideDocumentRangeFormattingEdits

▸ **provideDocumentRangeFormattingEdits**(`document`, `range`, `options`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TextEdit`](../classes/codearts_plugin_.TextEdit.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `range` | [`Range`](../classes/codearts_plugin_.Range.md) |  |
| `options` | [`FormattingOptions`](codearts_plugin_.FormattingOptions.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TextEdit`](../classes/codearts_plugin_.TextEdit.md)[]\>

#### Defined in

[index.d.ts:3965](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3965)
