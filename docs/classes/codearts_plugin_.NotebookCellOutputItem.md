[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookCellOutputItem

# Class: NotebookCellOutputItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookCellOutputItem

## Table of contents

### Constructors

- [constructor](codearts_plugin_.NotebookCellOutputItem.md#constructor)

### Properties

- [data](codearts_plugin_.NotebookCellOutputItem.md#data)
- [mime](codearts_plugin_.NotebookCellOutputItem.md#mime)

### Methods

- [error](codearts_plugin_.NotebookCellOutputItem.md#error)
- [json](codearts_plugin_.NotebookCellOutputItem.md#json)
- [stderr](codearts_plugin_.NotebookCellOutputItem.md#stderr)
- [stdout](codearts_plugin_.NotebookCellOutputItem.md#stdout)
- [text](codearts_plugin_.NotebookCellOutputItem.md#text)

## Constructors

### constructor

• **new NotebookCellOutputItem**(`data`, `mime`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `Uint8Array` |  |
| `mime` | `string` |  |

#### Defined in

[index.d.ts:13245](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13245)

## Properties

### data

• **data**: `Uint8Array`

#### Defined in

[index.d.ts:13237](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13237)

___

### mime

• **mime**: `string`

#### Defined in

[index.d.ts:13232](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13232)

## Methods

### error

▸ `Static` **error**(`value`): [`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `Error` |  |

#### Returns

[`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

#### Defined in

[index.d.ts:13223](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13223)

___

### json

▸ `Static` **json**(`value`, `mime?`): [`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` |  |
| `mime?` | `string` |  |

#### Returns

[`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

#### Defined in

[index.d.ts:13196](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13196)

___

### stderr

▸ `Static` **stderr**(`value`): [`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` |  |

#### Returns

[`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

#### Defined in

[index.d.ts:13214](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13214)

___

### stdout

▸ `Static` **stdout**(`value`): [`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` |  |

#### Returns

[`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

#### Defined in

[index.d.ts:13205](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13205)

___

### text

▸ `Static` **text**(`value`, `mime?`): [`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` |  |
| `mime?` | `string` |  |

#### Returns

[`NotebookCellOutputItem`](codearts_plugin_.NotebookCellOutputItem.md)

#### Defined in

[index.d.ts:13182](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13182)
