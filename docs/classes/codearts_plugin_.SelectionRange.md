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

[index.d.ts:5114](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L5114)

## Properties

### parent

• `Optional` **parent**: [`SelectionRange`](codearts_plugin_.SelectionRange.md)

The parent selection range containing this range.

#### Defined in

[index.d.ts:5106](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L5106)

___

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

The [Range](codearts_plugin_.Range.md) of this selection range.

#### Defined in

[index.d.ts:5101](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L5101)
