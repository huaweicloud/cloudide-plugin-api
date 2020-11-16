**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FoldingRange

# Class: FoldingRange

A line based folding range. To be valid, start and end line must be bigger than zero and smaller than the number of lines in the document.
Invalid ranges will be ignored.

## Hierarchy

* **FoldingRange**

## Index

### Constructors

* [constructor](_index_d_._plugin_.foldingrange.md#constructor)

### Properties

* [end](_index_d_._plugin_.foldingrange.md#end)
* [kind](_index_d_._plugin_.foldingrange.md#kind)
* [start](_index_d_._plugin_.foldingrange.md#start)

## Constructors

### constructor

\+ **new FoldingRange**(`start`: number, `end`: number, `kind?`: [FoldingRangeKind](../enums/_index_d_._plugin_.foldingrangekind.md)): [FoldingRange](_index_d_._plugin_.foldingrange.md)

*Defined in [index.d.ts:4191](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4191)*

Creates a new folding range.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`start` | number | The start line of the folded range. |
`end` | number | The end line of the folded range. |
`kind?` | [FoldingRangeKind](../enums/_index_d_._plugin_.foldingrangekind.md) | The kind of the folding range.  |

**Returns:** [FoldingRange](_index_d_._plugin_.foldingrange.md)

## Properties

### end

•  **end**: number

*Defined in [index.d.ts:4182](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4182)*

The zero-based end line of the range to fold. The folded area ends with the line's last character.
To be valid, the end must be zero or larger and smaller than the number of lines in the document.

___

### kind

• `Optional` **kind**: [FoldingRangeKind](../enums/_index_d_._plugin_.foldingrangekind.md)

*Defined in [index.d.ts:4191](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4191)*

Describes the [Kind](#FoldingRangeKind) of the folding range such as [Comment](#FoldingRangeKind.Comment) or
[Region](#FoldingRangeKind.Region). The kind is used to categorize folding ranges and used by commands
like 'Fold all comments'. See
[FoldingRangeKind](#FoldingRangeKind) for an enumeration of all kinds.
If not set, the range is originated from a syntax element.

___

### start

•  **start**: number

*Defined in [index.d.ts:4176](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4176)*

The zero-based start line of the range to fold. The folded area starts after the line's last character.
To be valid, the end must be zero or larger and smaller than the number of lines in the document.
