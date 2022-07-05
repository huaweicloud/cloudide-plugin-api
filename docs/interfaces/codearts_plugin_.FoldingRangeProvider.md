[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FoldingRangeProvider

# Interface: FoldingRangeProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).FoldingRangeProvider

## Table of contents

### Properties

- [onDidChangeFoldingRanges](codearts_plugin_.FoldingRangeProvider.md#ondidchangefoldingranges)

### Methods

- [provideFoldingRanges](codearts_plugin_.FoldingRangeProvider.md#providefoldingranges)

## Properties

### onDidChangeFoldingRanges

• `Optional` **onDidChangeFoldingRanges**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Defined in

[index.d.ts:5080](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L5080)

## Methods

### provideFoldingRanges

▸ **provideFoldingRanges**(`document`, `context`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`FoldingRange`](../classes/codearts_plugin_.FoldingRange.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `context` | [`FoldingContext`](codearts_plugin_.FoldingContext.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`FoldingRange`](../classes/codearts_plugin_.FoldingRange.md)[]\>

#### Defined in

[index.d.ts:5089](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L5089)
