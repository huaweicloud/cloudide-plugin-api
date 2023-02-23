[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Comment

# Interface: Comment

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Comment

A comment is displayed within the editor or the Comments Panel, depending on how it is provided.

## Table of contents

### Properties

- [author](cloudide_plugin_.Comment.md#author)
- [body](cloudide_plugin_.Comment.md#body)
- [contextValue](cloudide_plugin_.Comment.md#contextvalue)
- [label](cloudide_plugin_.Comment.md#label)
- [mode](cloudide_plugin_.Comment.md#mode)
- [reactions](cloudide_plugin_.Comment.md#reactions)

## Properties

### author

• **author**: [`CommentAuthorInformation`](cloudide_plugin_.CommentAuthorInformation.md)

The [author information](#CommentAuthorInformation) of the comment

#### Defined in

[index.d.ts:10951](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10951)

___

### body

• **body**: `string` \| [`MarkdownString`](../classes/cloudide_plugin_.MarkdownString.md)

The human-readable comment body

#### Defined in

[index.d.ts:10941](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10941)

___

### contextValue

• `Optional` **contextValue**: `string`

Context value of the comment. This can be used to contribute comment specific actions.
For example, a comment is given a context value as `editable`. When contributing actions to `comments/comment/title`
using `menus` extension point, you can specify context value for key `comment` in `when` expression like `comment == editable`.
```json
 "contributes": {
   "menus": {
     "comments/comment/title": [
       {
         "command": "extension.deleteComment",
         "when": "comment == editable"
       }
     ]
   }
 }
```
This will show action `extension.deleteComment` only for comments with `contextValue` is `editable`.

#### Defined in

[index.d.ts:10971](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10971)

___

### label

• `Optional` **label**: `string`

Optional label describing the [Comment](#Comment)
Label will be rendered next to authorName if exists.

#### Defined in

[index.d.ts:10982](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10982)

___

### mode

• **mode**: [`CommentMode`](../enums/cloudide_plugin_.CommentMode.md)

[Comment mode](#CommentMode) of the comment

#### Defined in

[index.d.ts:10946](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10946)

___

### reactions

• `Optional` **reactions**: [`CommentReaction`](cloudide_plugin_.CommentReaction.md)[]

Optional reactions of the [comment](#Comment)

#### Defined in

[index.d.ts:10976](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10976)
