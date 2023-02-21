[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SelectionRange

# Class: SelectionRange

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SelectionRange

A selection range represents a part of a selection hierarchy. A selection range
may have a parent selection range that contains it.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.SelectionRange.md#constructor)

### Properties

- [parent](cloudide_plugin_.SelectionRange.md#parent)
- [range](cloudide_plugin_.SelectionRange.md#range)

## Constructors

### constructor

• **new SelectionRange**(`range`, `parent?`)

Creates a new selection range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](cloudide_plugin_.Range.md) | The range of the selection range. |
| `parent?` | [`SelectionRange`](cloudide_plugin_.SelectionRange.md) | The parent of the selection range. |

#### Defined in

[index.d.ts:11111](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11111)

## Properties

### parent

• `Optional` **parent**: [`SelectionRange`](cloudide_plugin_.SelectionRange.md)

The parent selection range containing this range.

#### Defined in

[index.d.ts:11103](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11103)

___

### range

• **range**: [`Range`](cloudide_plugin_.Range.md)

The [range](#Range) of this selection range.

#### Defined in

[index.d.ts:11098](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11098)
