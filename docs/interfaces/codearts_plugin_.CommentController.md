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

[index.d.ts:14997](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14997)

___

### id

• `Readonly` **id**: `string`

#### Defined in

[index.d.ts:14980](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14980)

___

### label

• `Readonly` **label**: `string`

#### Defined in

[index.d.ts:14985](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14985)

___

### options

• `Optional` **options**: [`CommentOptions`](codearts_plugin_.CommentOptions.md)

#### Defined in

[index.d.ts:14990](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14990)

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

[index.d.ts:15007](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15007)

___

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:15020](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15020)

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

[index.d.ts:15012](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15012)
