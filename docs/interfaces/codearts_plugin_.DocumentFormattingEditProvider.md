[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentFormattingEditProvider

# Interface: DocumentFormattingEditProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentFormattingEditProvider

## Table of contents

### Methods

- [provideDocumentFormattingEdits](codearts_plugin_.DocumentFormattingEditProvider.md#providedocumentformattingedits)

## Methods

### provideDocumentFormattingEdits

▸ **provideDocumentFormattingEdits**(`document`, `options`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TextEdit`](../classes/codearts_plugin_.TextEdit.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `options` | [`FormattingOptions`](codearts_plugin_.FormattingOptions.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TextEdit`](../classes/codearts_plugin_.TextEdit.md)[]\>

#### Defined in

[index.d.ts:3942](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L3942)
