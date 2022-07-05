[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CommentController

# Interface: CommentController

["@codearts/plugin"](../modules/_codearts_plugin_.md).CommentController

## Table of contents

### Properties

- [commentingRangeProvider](codearts_plugin_.CommentController.md#commentingrangeprovider)
- [id](codearts_plugin_.CommentController.md#id)
- [label](codearts_plugin_.CommentController.md#label)
- [options](codearts_plugin_.CommentController.md#options)

### Methods

- [createCommentThread](codearts_plugin_.CommentController.md#createcommentthread)
- [dispose](codearts_plugin_.CommentController.md#dispose)
- [reactionHandler](codearts_plugin_.CommentController.md#reactionhandler)

## Properties

### commentingRangeProvider

• `Optional` **commentingRangeProvider**: [`CommentingRangeProvider`](codearts_plugin_.CommentingRangeProvider.md)

#### Defined in

[index.d.ts:14967](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L14967)

___

### id

• `Readonly` **id**: `string`

#### Defined in

[index.d.ts:14950](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L14950)

___

### label

• `Readonly` **label**: `string`

#### Defined in

[index.d.ts:14955](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L14955)

___

### options

• `Optional` **options**: [`CommentOptions`](codearts_plugin_.CommentOptions.md)

#### Defined in

[index.d.ts:14960](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L14960)

## Methods

### createCommentThread

▸ **createCommentThread**(`uri`, `range`, `comments`): [`CommentThread`](codearts_plugin_.CommentThread.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `range` | [`Range`](../classes/codearts_plugin_.Range.md) |  |
| `comments` | readonly [`Comment`](codearts_plugin_.Comment.md)[] |  |

#### Returns

[`CommentThread`](codearts_plugin_.CommentThread.md)

#### Defined in

[index.d.ts:14977](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L14977)

___

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:14990](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L14990)

___

### reactionHandler

▸ `Optional` **reactionHandler**(`comment`, `reaction`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `comment` | [`Comment`](codearts_plugin_.Comment.md) |
| `reaction` | [`CommentReaction`](codearts_plugin_.CommentReaction.md) |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:14982](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L14982)
