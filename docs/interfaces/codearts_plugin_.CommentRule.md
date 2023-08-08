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

[index.d.ts:5496](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5496)

___

### lineComment

• `Optional` **lineComment**: `string`

The line comment token, like `// this is a comment`

#### Defined in

[index.d.ts:5491](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5491)
