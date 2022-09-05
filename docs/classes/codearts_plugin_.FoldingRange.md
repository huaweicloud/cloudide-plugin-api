[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FoldingRange

# Class: FoldingRange

["@codearts/plugin"](../modules/_codearts_plugin_.md).FoldingRange

A line based folding range. To be valid, start and end line must be bigger than zero and smaller than the number of lines in the document.
Invalid ranges will be ignored.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.FoldingRange.md#constructor)

### Properties

- [end](codearts_plugin_.FoldingRange.md#end)
- [kind](codearts_plugin_.FoldingRange.md#kind)
- [start](codearts_plugin_.FoldingRange.md#start)

## Constructors

### constructor

• **new FoldingRange**(`start`, `end`, `kind?`)

Creates a new folding range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | `number` | The start line of the folded range. |
| `end` | `number` | The end line of the folded range. |
| `kind?` | [`FoldingRangeKind`](../enums/codearts_plugin_.FoldingRangeKind.md) | The kind of the folding range. |

#### Defined in

[index.d.ts:5041](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L5041)

## Properties

### end

• **end**: `number`

The zero-based end line of the range to fold. The folded area ends with the line's last character.
To be valid, the end must be zero or larger and smaller than the number of lines in the document.

#### Defined in

[index.d.ts:5023](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L5023)

___

### kind

• `Optional` **kind**: [`FoldingRangeKind`](../enums/codearts_plugin_.FoldingRangeKind.md)

Describes the [Kind](../enums/codearts_plugin_.FoldingRangeKind.md) of the folding range such as [Comment](../enums/codearts_plugin_.FoldingRangeKind.md#comment) or
[Region](../enums/codearts_plugin_.FoldingRangeKind.md#region). The kind is used to categorize folding ranges and used by commands
like 'Fold all comments'. See
[FoldingRangeKind](../enums/codearts_plugin_.FoldingRangeKind.md) for an enumeration of all kinds.
If not set, the range is originated from a syntax element.

#### Defined in

[index.d.ts:5032](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L5032)

___

### start

• **start**: `number`

The zero-based start line of the range to fold. The folded area starts after the line's last character.
To be valid, the end must be zero or larger and smaller than the number of lines in the document.

#### Defined in

[index.d.ts:5017](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L5017)
