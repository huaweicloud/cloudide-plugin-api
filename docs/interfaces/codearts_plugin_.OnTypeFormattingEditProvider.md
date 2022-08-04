[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / OnTypeFormattingEditProvider

# Interface: OnTypeFormattingEditProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).OnTypeFormattingEditProvider

## Table of contents

### Methods

- [provideOnTypeFormattingEdits](codearts_plugin_.OnTypeFormattingEditProvider.md#provideontypeformattingedits)

## Methods

### provideOnTypeFormattingEdits

▸ **provideOnTypeFormattingEdits**(`document`, `position`, `ch`, `options`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TextEdit`](../classes/codearts_plugin_.TextEdit.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `ch` | `string` |  |
| `options` | [`FormattingOptions`](codearts_plugin_.FormattingOptions.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TextEdit`](../classes/codearts_plugin_.TextEdit.md)[]\>

#### Defined in

[index.d.ts:3989](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L3989)
