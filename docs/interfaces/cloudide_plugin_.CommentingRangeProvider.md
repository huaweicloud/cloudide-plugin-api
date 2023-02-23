[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CommentingRangeProvider

# Interface: CommentingRangeProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CommentingRangeProvider

Commenting range provider for a [comment controller](#CommentController).

## Table of contents

### Methods

- [provideCommentingRanges](cloudide_plugin_.CommentingRangeProvider.md#providecommentingranges)

## Methods

### provideCommentingRanges

▸ **provideCommentingRanges**(`document`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`Range`](../classes/cloudide_plugin_.Range.md)[]\>

Provide a list of ranges which allow new comment threads creation or null for a given document

#### Parameters

| Name | Type |
| :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`Range`](../classes/cloudide_plugin_.Range.md)[]\>

#### Defined in

[index.d.ts:11007](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11007)
