**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CommentingRangeProvider

# Interface: CommentingRangeProvider

Commenting range provider for a [comment controller](#CommentController).

## Hierarchy

* **CommentingRangeProvider**

## Index

### Methods

* [provideCommentingRanges](_index_d_._plugin_.commentingrangeprovider.md#providecommentingranges)

## Methods

### provideCommentingRanges

▸ **provideCommentingRanges**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Range](../classes/_index_d_._plugin_.range.md)[]>

*Defined in [index.d.ts:10915](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10915)*

Provide a list of ranges which allow new comment threads creation or null for a given document

#### Parameters:

Name | Type |
------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[Range](../classes/_index_d_._plugin_.range.md)[]>
