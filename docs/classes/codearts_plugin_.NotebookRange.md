[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookRange

# Class: NotebookRange

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookRange

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | `number` |  |
| `end` | `number` |  |

#### Defined in

[index.d.ts:13156](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13156)

## Properties

### end

• `Readonly` **end**: `number`

#### Defined in

[index.d.ts:13142](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13142)

___

### isEmpty

• `Readonly` **isEmpty**: `boolean`

#### Defined in

[index.d.ts:13147](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13147)

___

### start

• `Readonly` **start**: `number`

#### Defined in

[index.d.ts:13137](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13137)

## Methods

### with

▸ **with**(`change`): [`NotebookRange`](codearts_plugin_.NotebookRange.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `change` | `Object` |  |
| `change.end?` | `number` | - |
| `change.start?` | `number` | - |

#### Returns

[`NotebookRange`](codearts_plugin_.NotebookRange.md)

#### Defined in

[index.d.ts:13165](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13165)
