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

[index.d.ts:5438](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L5438)

___

### lineComment

• `Optional` **lineComment**: `string`

The line comment token, like `// this is a comment`

#### Defined in

[index.d.ts:5433](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L5433)
