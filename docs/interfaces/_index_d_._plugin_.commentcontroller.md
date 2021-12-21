**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CommentController

# Interface: CommentController

A comment controller is able to provide [comments](#CommentThread) support to the editor and
provide users various ways to interact with comments.

## Hierarchy

* **CommentController**

## Index

### Properties

* [commentingRangeProvider](_index_d_._plugin_.commentcontroller.md#commentingrangeprovider)
* [id](_index_d_._plugin_.commentcontroller.md#id)
* [label](_index_d_._plugin_.commentcontroller.md#label)
* [options](_index_d_._plugin_.commentcontroller.md#options)
* [reactionHandler](_index_d_._plugin_.commentcontroller.md#reactionhandler)

### Methods

* [createCommentThread](_index_d_._plugin_.commentcontroller.md#createcommentthread)
* [dispose](_index_d_._plugin_.commentcontroller.md#dispose)

## Properties

### commentingRangeProvider

• `Optional` **commentingRangeProvider**: [CommentingRangeProvider](_index_d_._plugin_.commentingrangeprovider.md)

*Defined in [index.d.ts:12412](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12412)*

Optional commenting range provider. Provide a list [ranges](#Range) which support commenting to any given resource uri.

If not provided, users can leave comments in any document opened in the editor.

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:12395](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12395)*

The id of this comment controller.

___

### label

• `Readonly` **label**: string

*Defined in [index.d.ts:12400](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12400)*

The human-readable label of this comment controller.

___

### options

• `Optional` **options**: [CommentOptions](_index_d_._plugin_.commentoptions.md)

*Defined in [index.d.ts:12405](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12405)*

Comment controller options

___

### reactionHandler

• `Optional` **reactionHandler**: (comment: [Comment](_index_d_._plugin_.comment.md), reaction: [CommentReaction](_index_d_._plugin_.commentreaction.md)) => [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:12427](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12427)*

Optional reaction handler for creating and deleting reactions on a [comment](#Comment).

## Methods

### createCommentThread

▸ **createCommentThread**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md), `range`: [Range](../classes/_index_d_._plugin_.range.md), `comments`: [Comment](_index_d_._plugin_.comment.md)[]): [CommentThread](_index_d_._plugin_.commentthread.md)

*Defined in [index.d.ts:12422](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12422)*

Create a [comment thread](#CommentThread). The comment thread will be displayed in visible text editors (if the resource matches)
and Comments Panel once created.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the document the thread has been created on. |
`range` | [Range](../classes/_index_d_._plugin_.range.md) | The range the comment thread is located within the document. |
`comments` | [Comment](_index_d_._plugin_.comment.md)[] | The ordered comments of the thread.  |

**Returns:** [CommentThread](_index_d_._plugin_.commentthread.md)

___

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:12435](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12435)*

Dispose this comment controller.

Once disposed, all [comment threads](#CommentThread) created by this comment controller will also be removed from the editor
and Comments Panel.

**Returns:** void
