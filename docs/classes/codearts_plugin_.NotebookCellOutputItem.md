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

[index.d.ts:13215](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13215)

## Properties

### data

• **data**: `Uint8Array`

#### Defined in

[index.d.ts:13207](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13207)

___

### mime

• **mime**: `string`

#### Defined in

[index.d.ts:13202](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13202)

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

[index.d.ts:13193](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13193)

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

[index.d.ts:13166](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13166)

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

[index.d.ts:13184](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13184)

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

[index.d.ts:13175](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13175)

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

[index.d.ts:13152](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13152)
