[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CommentReaction

# Interface: CommentReaction

["@codearts/plugin"](../modules/_codearts_plugin_.md).CommentReaction

Reactions of a [Comment](codearts_plugin_.Comment.md)

## Table of contents

### Properties

- [authorHasReacted](codearts_plugin_.CommentReaction.md#authorhasreacted)
- [count](codearts_plugin_.CommentReaction.md#count)
- [iconPath](codearts_plugin_.CommentReaction.md#iconpath)
- [label](codearts_plugin_.CommentReaction.md#label)

## Properties

### authorHasReacted

• `Readonly` **authorHasReacted**: `boolean`

Whether the [author](codearts_plugin_.CommentAuthorInformation.md) of the comment has reacted to this reaction

#### Defined in

[index.d.ts:15271](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15271)

___

### count

• `Readonly` **count**: `number`

The number of users who have reacted to this reaction

#### Defined in

[index.d.ts:15266](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15266)

___

### iconPath

• `Readonly` **iconPath**: `string` \| [`Uri`](../classes/codearts_plugin_.Uri.md)

Icon for the reaction shown in UI.

#### Defined in

[index.d.ts:15261](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15261)

___

### label

• `Readonly` **label**: `string`

The human-readable label for the reaction

#### Defined in

[index.d.ts:15256](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15256)
