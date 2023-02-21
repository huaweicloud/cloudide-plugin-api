[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CommentReaction

# Interface: CommentReaction

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CommentReaction

Reactions of a [comment](#Comment)

## Table of contents

### Properties

- [authorHasReacted](cloudide_plugin_.CommentReaction.md#authorhasreacted)
- [count](cloudide_plugin_.CommentReaction.md#count)
- [iconPath](cloudide_plugin_.CommentReaction.md#iconpath)
- [label](cloudide_plugin_.CommentReaction.md#label)

## Properties

### authorHasReacted

• `Readonly` **authorHasReacted**: `boolean`

Whether the [author](CommentAuthorInformation) of the comment has reacted to this reaction

#### Defined in

[index.d.ts:10931](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10931)

___

### count

• `Readonly` **count**: `number`

The number of users who have reacted to this reaction

#### Defined in

[index.d.ts:10926](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10926)

___

### iconPath

• `Readonly` **iconPath**: `string` \| [`Uri`](../classes/cloudide_plugin_.Uri.md)

Icon for the reaction shown in UI.

#### Defined in

[index.d.ts:10921](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10921)

___

### label

• `Readonly` **label**: `string`

The human-readable label for the reaction

#### Defined in

[index.d.ts:10916](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10916)
