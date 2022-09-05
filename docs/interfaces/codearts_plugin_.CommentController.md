[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CommentController

# Interface: CommentController

["@codearts/plugin"](../modules/_codearts_plugin_.md).CommentController

A comment controller is able to provide [comments](codearts_plugin_.CommentThread.md) support to the editor and
provide users various ways to interact with comments.

## Table of contents

### Properties

- [commentingRangeProvider](codearts_plugin_.CommentController.md#commentingrangeprovider)
- [id](codearts_plugin_.CommentController.md#id)
- [label](codearts_plugin_.CommentController.md#label)
- [options](codearts_plugin_.CommentController.md#options)
- [reactionHandler](codearts_plugin_.CommentController.md#reactionhandler)

### Methods

- [createCommentThread](codearts_plugin_.CommentController.md#createcommentthread)
- [dispose](codearts_plugin_.CommentController.md#dispose)

## Properties

### commentingRangeProvider

• `Optional` **commentingRangeProvider**: [`CommentingRangeProvider`](codearts_plugin_.CommentingRangeProvider.md)

Optional commenting range provider. Provide a list [ranges](../classes/codearts_plugin_.Range.md) which support commenting to any given resource uri.

If not provided, users can leave comments in any document opened in the editor.

#### Defined in

[index.d.ts:15059](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15059)

___

### id

• `Readonly` **id**: `string`

The id of this comment controller.

#### Defined in

[index.d.ts:15042](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15042)

___

### label

• `Readonly` **label**: `string`

The human-readable label of this comment controller.

#### Defined in

[index.d.ts:15047](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15047)

___

### options

• `Optional` **options**: [`CommentOptions`](codearts_plugin_.CommentOptions.md)

Comment controller options

#### Defined in

[index.d.ts:15052](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15052)

___

### reactionHandler

• `Optional` **reactionHandler**: (`comment`: [`Comment`](codearts_plugin_.Comment.md), `reaction`: [`CommentReaction`](codearts_plugin_.CommentReaction.md)) => [`Thenable`](Thenable.md)<`void`\>

#### Type declaration

▸ (`comment`, `reaction`): [`Thenable`](Thenable.md)<`void`\>

Optional reaction handler for creating and deleting reactions on a [Comment](codearts_plugin_.Comment.md).

##### Parameters

| Name | Type |
| :------ | :------ |
| `comment` | [`Comment`](codearts_plugin_.Comment.md) |
| `reaction` | [`CommentReaction`](codearts_plugin_.CommentReaction.md) |

##### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:15074](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15074)

## Methods

### createCommentThread

▸ **createCommentThread**(`uri`, `range`, `comments`): [`CommentThread`](codearts_plugin_.CommentThread.md)

Create a [comment thread](codearts_plugin_.CommentThread.md). The comment thread will be displayed in visible text editors (if the resource matches)
and Comments Panel once created.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The uri of the document the thread has been created on. |
| `range` | [`Range`](../classes/codearts_plugin_.Range.md) | The range the comment thread is located within the document. |
| `comments` | readonly [`Comment`](codearts_plugin_.Comment.md)[] | The ordered comments of the thread. |

#### Returns

[`CommentThread`](codearts_plugin_.CommentThread.md)

#### Defined in

[index.d.ts:15069](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15069)

___

### dispose

▸ **dispose**(): `void`

Dispose this comment controller.

Once disposed, all [comment threads](codearts_plugin_.CommentThread.md) created by this comment controller will also be removed from the editor
and Comments Panel.

#### Returns

`void`

#### Defined in

[index.d.ts:15082](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15082)
