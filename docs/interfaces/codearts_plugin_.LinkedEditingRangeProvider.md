[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / LinkedEditingRangeProvider

# Interface: LinkedEditingRangeProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).LinkedEditingRangeProvider

## Table of contents

### Methods

- [provideLinkedEditingRanges](codearts_plugin_.LinkedEditingRangeProvider.md#providelinkededitingranges)

## Methods

### provideLinkedEditingRanges

▸ **provideLinkedEditingRanges**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`LinkedEditingRanges`](../classes/codearts_plugin_.LinkedEditingRanges.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`LinkedEditingRanges`](../classes/codearts_plugin_.LinkedEditingRanges.md)\>

#### Defined in

[index.d.ts:5416](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L5416)
