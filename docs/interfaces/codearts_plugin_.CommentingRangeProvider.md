[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CommentingRangeProvider

# Interface: CommentingRangeProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).CommentingRangeProvider

Commenting range provider for a [comment controller](codearts_plugin_.CommentController.md).

## Table of contents

### Methods

- [provideCommentingRanges](codearts_plugin_.CommentingRangeProvider.md#providecommentingranges)

## Methods

### provideCommentingRanges

▸ **provideCommentingRanges**(`document`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Range`](../classes/codearts_plugin_.Range.md)[]\>

Provide a list of ranges which allow new comment threads creation or null for a given document

#### Parameters

| Name | Type |
| :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Range`](../classes/codearts_plugin_.Range.md)[]\>

#### Defined in

[index.d.ts:15353](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15353)
