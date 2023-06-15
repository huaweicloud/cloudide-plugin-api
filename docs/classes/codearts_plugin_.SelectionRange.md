[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SelectionRange

# Class: SelectionRange

["@codearts/plugin"](../modules/_codearts_plugin_.md).SelectionRange

A selection range represents a part of a selection hierarchy. A selection range
may have a parent selection range that contains it.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.SelectionRange.md#constructor)

### Properties

- [parent](codearts_plugin_.SelectionRange.md#parent)
- [range](codearts_plugin_.SelectionRange.md#range)

## Constructors

### constructor

• **new SelectionRange**(`range`, `parent?`)

Creates a new selection range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) | The range of the selection range. |
| `parent?` | [`SelectionRange`](codearts_plugin_.SelectionRange.md) | The parent of the selection range. |

#### Defined in

[index.d.ts:5134](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5134)

## Properties

### parent

• `Optional` **parent**: [`SelectionRange`](codearts_plugin_.SelectionRange.md)

The parent selection range containing this range.

#### Defined in

[index.d.ts:5126](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5126)

___

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

The [Range](codearts_plugin_.Range.md) of this selection range.

#### Defined in

[index.d.ts:5121](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5121)
