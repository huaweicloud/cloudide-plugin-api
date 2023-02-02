[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CommentThread

# Interface: CommentThread

["@codearts/plugin"](../modules/_codearts_plugin_.md).CommentThread

A collection of [comments](codearts_plugin_.Comment.md) representing a conversation at a particular range in a document.

## Table of contents

### Properties

- [canReply](codearts_plugin_.CommentThread.md#canreply)
- [collapsibleState](codearts_plugin_.CommentThread.md#collapsiblestate)
- [comments](codearts_plugin_.CommentThread.md#comments)
- [contextValue](codearts_plugin_.CommentThread.md#contextvalue)
- [label](codearts_plugin_.CommentThread.md#label)
- [range](codearts_plugin_.CommentThread.md#range)
- [uri](codearts_plugin_.CommentThread.md#uri)

### Methods

- [dispose](codearts_plugin_.CommentThread.md#dispose)

## Properties

### canReply

• **canReply**: `boolean`

Whether the thread supports reply.
Defaults to true.

#### Defined in

[index.d.ts:15199](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15199)

___

### collapsibleState

• **collapsibleState**: [`CommentThreadCollapsibleState`](../enums/codearts_plugin_.CommentThreadCollapsibleState.md)

Whether the thread should be collapsed or expanded when opening the document.
Defaults to Collapsed.

#### Defined in

[index.d.ts:15193](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15193)

___

### comments

• **comments**: readonly [`Comment`](codearts_plugin_.Comment.md)[]

The ordered comments of the thread.

#### Defined in

[index.d.ts:15187](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15187)

___

### contextValue

• `Optional` **contextValue**: `string`

Context value of the comment thread. This can be used to contribute thread specific actions.
For example, a comment thread is given a context value as `editable`. When contributing actions to `comments/commentThread/title`
using `menus` extension point, you can specify context value for key `commentThread` in `when` expression like `commentThread == editable`.
```json
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

#### Defined in

[index.d.ts:15219](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15219)

___

### label

• `Optional` **label**: `string`

The optional human-readable label describing the [Comment Thread](codearts_plugin_.CommentThread.md)

#### Defined in

[index.d.ts:15224](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15224)

___

### range

• **range**: [`Range`](../classes/codearts_plugin_.Range.md)

The range the comment thread is located within the document. The thread icon will be shown
at the last line of the range.

#### Defined in

[index.d.ts:15182](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15182)

___

### uri

• `Readonly` **uri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The uri of the document the thread has been created on.

#### Defined in

[index.d.ts:15176](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15176)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose this comment thread.

Once disposed, this comment thread will be removed from visible editors and Comment Panel when appropriate.

#### Returns

`void`

#### Defined in

[index.d.ts:15231](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15231)
