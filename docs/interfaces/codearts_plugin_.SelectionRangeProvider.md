[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SelectionRangeProvider

# Interface: SelectionRangeProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).SelectionRangeProvider

## Table of contents

### Methods

- [provideSelectionRanges](codearts_plugin_.SelectionRangeProvider.md#provideselectionranges)

## Methods

### provideSelectionRanges

▸ **provideSelectionRanges**(`document`, `positions`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SelectionRange`](../classes/codearts_plugin_.SelectionRange.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `positions` | readonly [`Position`](../classes/codearts_plugin_.Position.md)[] |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`SelectionRange`](../classes/codearts_plugin_.SelectionRange.md)[]\>

#### Defined in

[index.d.ts:5131](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L5131)
