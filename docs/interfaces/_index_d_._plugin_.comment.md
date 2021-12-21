**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Comment

# Interface: Comment

A comment is displayed within the editor or the Comments Panel, depending on how it is provided.

## Hierarchy

* **Comment**

## Index

### Properties

* [author](_index_d_._plugin_.comment.md#author)
* [body](_index_d_._plugin_.comment.md#body)
* [contextValue](_index_d_._plugin_.comment.md#contextvalue)
* [label](_index_d_._plugin_.comment.md#label)
* [mode](_index_d_._plugin_.comment.md#mode)
* [reactions](_index_d_._plugin_.comment.md#reactions)

## Properties

### author

•  **author**: [CommentAuthorInformation](_index_d_._plugin_.commentauthorinformation.md)

*Defined in [index.d.ts:12313](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12313)*

The [author information](#CommentAuthorInformation) of the comment

___

### body

•  **body**: string \| [MarkdownString](../classes/_index_d_._plugin_.markdownstring.md)

*Defined in [index.d.ts:12303](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12303)*

The human-readable comment body

___

### contextValue

• `Optional` **contextValue**: string

*Defined in [index.d.ts:12333](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12333)*

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

___

### label

• `Optional` **label**: string

*Defined in [index.d.ts:12344](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12344)*

Optional label describing the [Comment](#Comment)
Label will be rendered next to authorName if exists.

___

### mode

•  **mode**: [CommentMode](../enums/_index_d_._plugin_.commentmode.md)

*Defined in [index.d.ts:12308](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12308)*

[Comment mode](#CommentMode) of the comment

___

### reactions

• `Optional` **reactions**: [CommentReaction](_index_d_._plugin_.commentreaction.md)[]

*Defined in [index.d.ts:12338](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L12338)*

Optional reactions of the [comment](#Comment)
