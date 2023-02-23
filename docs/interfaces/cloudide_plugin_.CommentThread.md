[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CommentThread

# Interface: CommentThread

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CommentThread

A collection of [comments](#Comment) representing a conversation at a particular range in a document.

## Table of contents

### Properties

- [collapsibleState](cloudide_plugin_.CommentThread.md#collapsiblestate)
- [comments](cloudide_plugin_.CommentThread.md#comments)
- [contextValue](cloudide_plugin_.CommentThread.md#contextvalue)
- [label](cloudide_plugin_.CommentThread.md#label)
- [range](cloudide_plugin_.CommentThread.md#range)
- [uri](cloudide_plugin_.CommentThread.md#uri)

### Methods

- [dispose](cloudide_plugin_.CommentThread.md#dispose)

## Properties

### collapsibleState

• **collapsibleState**: [`CommentThreadCollapsibleState`](../enums/cloudide_plugin_.CommentThreadCollapsibleState.md)

Whether the thread should be collapsed or expanded when opening the document.
Defaults to Collapsed.

#### Defined in

[index.d.ts:10859](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10859)

___

### comments

• **comments**: readonly [`Comment`](cloudide_plugin_.Comment.md)[]

The ordered comments of the thread.

#### Defined in

[index.d.ts:10853](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10853)

___

### contextValue

• `Optional` **contextValue**: `string`

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

#### Defined in

[index.d.ts:10879](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10879)

___

### label

• `Optional` **label**: `string`

The optional human-readable label describing the [Comment Thread](#CommentThread)

#### Defined in

[index.d.ts:10884](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10884)

___

### range

• **range**: [`Range`](../classes/cloudide_plugin_.Range.md)

The range the comment thread is located within the document. The thread icon will be shown
at the first line of the range.

#### Defined in

[index.d.ts:10848](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10848)

___

### uri

• `Readonly` **uri**: [`Uri`](../classes/cloudide_plugin_.Uri.md)

The uri of the document the thread has been created on.

#### Defined in

[index.d.ts:10842](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10842)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose this comment thread.

Once disposed, this comment thread will be removed from visible editors and Comment Panel when appropriate.

#### Returns

`void`

#### Defined in

[index.d.ts:10891](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10891)
