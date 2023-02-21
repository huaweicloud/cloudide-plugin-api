[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CommentController

# Interface: CommentController

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CommentController

A comment controller is able to provide [comments](#CommentThread) support to the editor and
provide users various ways to interact with comments.

## Table of contents

### Properties

- [commentingRangeProvider](cloudide_plugin_.CommentController.md#commentingrangeprovider)
- [id](cloudide_plugin_.CommentController.md#id)
- [label](cloudide_plugin_.CommentController.md#label)
- [options](cloudide_plugin_.CommentController.md#options)
- [reactionHandler](cloudide_plugin_.CommentController.md#reactionhandler)

### Methods

- [createCommentThread](cloudide_plugin_.CommentController.md#createcommentthread)
- [dispose](cloudide_plugin_.CommentController.md#dispose)

## Properties

### commentingRangeProvider

• `Optional` **commentingRangeProvider**: [`CommentingRangeProvider`](cloudide_plugin_.CommentingRangeProvider.md)

Optional commenting range provider. Provide a list [ranges](#Range) which support commenting to any given resource uri.

If not provided, users can leave comments in any document opened in the editor.

#### Defined in

[index.d.ts:11050](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11050)

___

### id

• `Readonly` **id**: `string`

The id of this comment controller.

#### Defined in

[index.d.ts:11033](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11033)

___

### label

• `Readonly` **label**: `string`

The human-readable label of this comment controller.

#### Defined in

[index.d.ts:11038](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11038)

___

### options

• `Optional` **options**: [`CommentOptions`](cloudide_plugin_.CommentOptions.md)

Comment controller options

#### Defined in

[index.d.ts:11043](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11043)

___

### reactionHandler

• `Optional` **reactionHandler**: (`comment`: [`Comment`](cloudide_plugin_.Comment.md), `reaction`: [`CommentReaction`](cloudide_plugin_.CommentReaction.md)) => `Promise`<`void`\>

#### Type declaration

▸ (`comment`, `reaction`): `Promise`<`void`\>

Optional reaction handler for creating and deleting reactions on a [comment](#Comment).

##### Parameters

| Name | Type |
| :------ | :------ |
| `comment` | [`Comment`](cloudide_plugin_.Comment.md) |
| `reaction` | [`CommentReaction`](cloudide_plugin_.CommentReaction.md) |

##### Returns

`Promise`<`void`\>

#### Defined in

[index.d.ts:11065](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11065)

## Methods

### createCommentThread

▸ **createCommentThread**(`uri`, `range`, `comments`): [`CommentThread`](cloudide_plugin_.CommentThread.md)

Create a [comment thread](#CommentThread). The comment thread will be displayed in visible text editors (if the resource matches)
and Comments Panel once created.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The uri of the document the thread has been created on. |
| `range` | [`Range`](../classes/cloudide_plugin_.Range.md) | The range the comment thread is located within the document. |
| `comments` | [`Comment`](cloudide_plugin_.Comment.md)[] | The ordered comments of the thread. |

#### Returns

[`CommentThread`](cloudide_plugin_.CommentThread.md)

#### Defined in

[index.d.ts:11060](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11060)

___

### dispose

▸ **dispose**(): `void`

Dispose this comment controller.

Once disposed, all [comment threads](#CommentThread) created by this comment controller will also be removed from the editor
and Comments Panel.

#### Returns

`void`

#### Defined in

[index.d.ts:11073](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11073)
