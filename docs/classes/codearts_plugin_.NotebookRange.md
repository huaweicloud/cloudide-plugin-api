[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookRange

# Class: NotebookRange

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookRange

A notebook range represents an ordered pair of two cell indices.
It is guaranteed that start is less than or equal to end.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.NotebookRange.md#constructor)

### Properties

- [end](codearts_plugin_.NotebookRange.md#end)
- [isEmpty](codearts_plugin_.NotebookRange.md#isempty)
- [start](codearts_plugin_.NotebookRange.md#start)

### Methods

- [with](codearts_plugin_.NotebookRange.md#with)

## Constructors

### constructor

• **new NotebookRange**(`start`, `end`)

Create a new notebook range. If `start` is not
before or equal to `end`, the values will be swapped.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | `number` | start index |
| `end` | `number` | end index. |

#### Defined in

[index.d.ts:13218](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13218)

## Properties

### end

• `Readonly` **end**: `number`

The exclusive end index of this range (zero-based).

#### Defined in

[index.d.ts:13204](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13204)

___

### isEmpty

• `Readonly` **isEmpty**: `boolean`

`true` if `start` and `end` are equal.

#### Defined in

[index.d.ts:13209](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13209)

___

### start

• `Readonly` **start**: `number`

The zero-based start index of this range.

#### Defined in

[index.d.ts:13199](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13199)

## Methods

### with

▸ **with**(`change`): [`NotebookRange`](codearts_plugin_.NotebookRange.md)

Derive a new range for this range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `change` | `Object` | An object that describes a change to this range. |
| `change.end?` | `number` | - |
| `change.start?` | `number` | - |

#### Returns

[`NotebookRange`](codearts_plugin_.NotebookRange.md)

A range that reflects the given change. Will return `this` range if the change
is not changing anything.

#### Defined in

[index.d.ts:13227](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13227)
