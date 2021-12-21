**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CommentThread

# Interface: CommentThread

A collection of [comments](#Comment) representing a conversation at a particular range in a document.

## Hierarchy

* **CommentThread**

## Index

### Properties

* [canReply](_index_d_._plugin_.commentthread.md#canreply)
* [collapsibleState](_index_d_._plugin_.commentthread.md#collapsiblestate)
* [comments](_index_d_._plugin_.commentthread.md#comments)
* [contextValue](_index_d_._plugin_.commentthread.md#contextvalue)
* [label](_index_d_._plugin_.commentthread.md#label)
* [range](_index_d_._plugin_.commentthread.md#range)
* [uri](_index_d_._plugin_.commentthread.md#uri)

### Methods

* [dispose](_index_d_._plugin_.commentthread.md#dispose)

## Properties

### canReply

•  **canReply**: boolean

*Defined in [index.d.ts:12221](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12221)*

Whether the thread supports reply.
Defaults to true.

___

### collapsibleState

•  **collapsibleState**: [CommentThreadCollapsibleState](../enums/_index_d_._plugin_.commentthreadcollapsiblestate.md)

*Defined in [index.d.ts:12215](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12215)*

Whether the thread should be collapsed or expanded when opening the document.
Defaults to Collapsed.

___

### comments

•  **comments**: ReadonlyArray\<[Comment](_index_d_._plugin_.comment.md)>

*Defined in [index.d.ts:12209](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12209)*

The ordered comments of the thread.

___

### contextValue

• `Optional` **contextValue**: string

*Defined in [index.d.ts:12241](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12241)*

Context value of the comment thread. This can be used to contribute thread specific actions.
For example, a comment thread is given a context value as `editable`. When contributing actions to `comments/commentThread/title`
using `menus` extension point, you can specify context value for key `commentThread` in `when` expression like `commentThread == editable`.
```
	"contributes": {
		"menus": {
			"comments/commentThread/title": [
				{
					"command": "extension.deleteCommentThread",
					"when": "commentThread == editable"
				}
			]
		}
	}
```
This will show action `extension.deleteCommentThread` only for comment threads with `contextValue` is `editable`.

___

### label

• `Optional` **label**: string

*Defined in [index.d.ts:12246](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12246)*

The optional human-readable label describing the [Comment Thread](#CommentThread)

___

### range

•  **range**: [Range](../classes/_index_d_._plugin_.range.md)

*Defined in [index.d.ts:12204](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12204)*

The range the comment thread is located within the document. The thread icon will be shown
at the first line of the range.

___

### uri

• `Readonly` **uri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:12198](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12198)*

The uri of the document the thread has been created on.

## Methods

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:12253](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12253)*

Dispose this comment thread.

Once disposed, this comment thread will be removed from visible editors and Comment Panel when appropriate.

**Returns:** void
