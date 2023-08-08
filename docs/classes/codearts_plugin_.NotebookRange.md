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

[index.d.ts:14091](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14091)

## Properties

### end

• `Readonly` **end**: `number`

The exclusive end index of this range (zero-based).

#### Defined in

[index.d.ts:14077](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14077)

___

### isEmpty

• `Readonly` **isEmpty**: `boolean`

`true` if `start` and `end` are equal.

#### Defined in

[index.d.ts:14082](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14082)

___

### start

• `Readonly` **start**: `number`

The zero-based start index of this range.

#### Defined in

[index.d.ts:14072](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14072)

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

[index.d.ts:14100](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14100)
