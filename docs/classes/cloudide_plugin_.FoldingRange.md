[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / FoldingRange

# Class: FoldingRange

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).FoldingRange

A line based folding range. To be valid, start and end line must a zero or larger and smaller than the number of lines in the document.
Invalid ranges will be ignored.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.FoldingRange.md#constructor)

### Properties

- [end](cloudide_plugin_.FoldingRange.md#end)
- [kind](cloudide_plugin_.FoldingRange.md#kind)
- [start](cloudide_plugin_.FoldingRange.md#start)

## Constructors

### constructor

• **new FoldingRange**(`start`, `end`, `kind?`)

Creates a new folding range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | `number` | The start line of the folded range. |
| `end` | `number` | The end line of the folded range. |
| `kind?` | [`FoldingRangeKind`](../enums/cloudide_plugin_.FoldingRangeKind.md) | The kind of the folding range. |

#### Defined in

[index.d.ts:7265](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7265)

## Properties

### end

• **end**: `number`

The zero-based end line of the range to fold. The folded area ends with the line's last character.
To be valid, the end must be zero or larger and smaller than the number of lines in the document.

#### Defined in

[index.d.ts:7247](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7247)

___

### kind

• `Optional` **kind**: [`FoldingRangeKind`](../enums/cloudide_plugin_.FoldingRangeKind.md)

Describes the [Kind](#FoldingRangeKind) of the folding range such as [Comment](#FoldingRangeKind.Comment) or
[Region](#FoldingRangeKind.Region). The kind is used to categorize folding ranges and used by commands
like 'Fold all comments'. See
[FoldingRangeKind](#FoldingRangeKind) for an enumeration of all kinds.
If not set, the range is originated from a syntax element.

#### Defined in

[index.d.ts:7256](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7256)

___

### start

• **start**: `number`

The zero-based start line of the range to fold. The folded area starts after the line's last character.
To be valid, the end must be zero or larger and smaller than the number of lines in the document.

#### Defined in

[index.d.ts:7241](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7241)
