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

[index.d.ts:15585](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15585)

___

### collapsibleState

• **collapsibleState**: [`CommentThreadCollapsibleState`](../enums/codearts_plugin_.CommentThreadCollapsibleState.md)

Whether the thread should be collapsed or expanded when opening the document.
Defaults to Collapsed.

#### Defined in

[index.d.ts:15579](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15579)

___

### comments

• **comments**: readonly [`Comment`](codearts_plugin_.Comment.md)[]

The ordered comments of the thread.

#### Defined in

[index.d.ts:15573](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15573)

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

[index.d.ts:15605](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15605)

___

### label

• `Optional` **label**: `string`

The optional human-readable label describing the [Comment Thread](codearts_plugin_.CommentThread.md)

#### Defined in

[index.d.ts:15610](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15610)

___

### range

• **range**: [`Range`](../classes/codearts_plugin_.Range.md)

The range the comment thread is located within the document. The thread icon will be shown
at the last line of the range.

#### Defined in

[index.d.ts:15568](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15568)

___

### uri

• `Readonly` **uri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The uri of the document the thread has been created on.

#### Defined in

[index.d.ts:15562](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15562)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose this comment thread.

Once disposed, this comment thread will be removed from visible editors and Comment Panel when appropriate.

#### Returns

`void`

#### Defined in

[index.d.ts:15617](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15617)
