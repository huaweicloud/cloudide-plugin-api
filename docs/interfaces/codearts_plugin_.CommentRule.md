[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CommentRule

# Interface: CommentRule

["@codearts/plugin"](../modules/_codearts_plugin_.md).CommentRule

Describes how comments for a language work.

## Table of contents

### Properties

- [blockComment](codearts_plugin_.CommentRule.md#blockcomment)
- [lineComment](codearts_plugin_.CommentRule.md#linecomment)

## Properties

### blockComment

• `Optional` **blockComment**: [`CharacterPair`](../modules/_codearts_plugin_.md#characterpair)

The block comment character pair, like `/* block comment *&#47;`

#### Defined in

[index.d.ts:5509](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5509)

___

### lineComment

• `Optional` **lineComment**: `string`

The line comment token, like `// this is a comment`

#### Defined in

[index.d.ts:5504](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5504)
