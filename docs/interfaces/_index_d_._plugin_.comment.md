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

*Defined in [index.d.ts:12345](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L12345)*

The [author information](#CommentAuthorInformation) of the comment

___

### body

•  **body**: string \| [MarkdownString](../classes/_index_d_._plugin_.markdownstring.md)

*Defined in [index.d.ts:12335](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L12335)*

The human-readable comment body

___

### contextValue

• `Optional` **contextValue**: string

*Defined in [index.d.ts:12365](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L12365)*

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

*Defined in [index.d.ts:12376](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L12376)*

Optional label describing the [Comment](#Comment)
Label will be rendered next to authorName if exists.

___

### mode

•  **mode**: [CommentMode](../enums/_index_d_._plugin_.commentmode.md)

*Defined in [index.d.ts:12340](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L12340)*

[Comment mode](#CommentMode) of the comment

___

### reactions

• `Optional` **reactions**: [CommentReaction](_index_d_._plugin_.commentreaction.md)[]

*Defined in [index.d.ts:12370](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L12370)*

Optional reactions of the [comment](#Comment)
