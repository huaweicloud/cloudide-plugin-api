**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CommentRule

# Interface: CommentRule

Describes how comments for a language work.

## Hierarchy

* **CommentRule**

## Index

### Properties

* [blockComment](_index_d_._plugin_.commentrule.md#blockcomment)
* [lineComment](_index_d_._plugin_.commentrule.md#linecomment)

## Properties

### blockComment

• `Optional` **blockComment**: [CharacterPair](../modules/_index_d_._plugin_.md#characterpair)

*Defined in [index.d.ts:4742](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L4742)*

The block comment character pair, like `/* block comment *&#47;`

___

### lineComment

• `Optional` **lineComment**: string

*Defined in [index.d.ts:4737](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L4737)*

The line comment token, like `// this is a comment`
