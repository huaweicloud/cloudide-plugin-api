**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CommentReaction

# Interface: CommentReaction

Reactions of a [comment](#Comment)

## Hierarchy

* **CommentReaction**

## Index

### Properties

* [authorHasReacted](_index_d_._plugin_.commentreaction.md#authorhasreacted)
* [count](_index_d_._plugin_.commentreaction.md#count)
* [iconPath](_index_d_._plugin_.commentreaction.md#iconpath)
* [label](_index_d_._plugin_.commentreaction.md#label)

## Properties

### authorHasReacted

• `Readonly` **authorHasReacted**: boolean

*Defined in [index.d.ts:10839](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10839)*

Whether the [author](CommentAuthorInformation) of the comment has reacted to this reaction

___

### count

• `Readonly` **count**: number

*Defined in [index.d.ts:10834](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10834)*

The number of users who have reacted to this reaction

___

### iconPath

• `Readonly` **iconPath**: string \| [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:10829](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10829)*

Icon for the reaction shown in UI.

___

### label

• `Readonly` **label**: string

*Defined in [index.d.ts:10824](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10824)*

The human-readable label for the reaction
