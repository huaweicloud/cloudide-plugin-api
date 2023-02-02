[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookData

# Class: NotebookData

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookData

Raw representation of a notebook.

Extensions are responsible for creating [`NotebookData`](codearts_plugin_.NotebookData.md) so that the editor
can create a [`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md).

**`See`**

[NotebookSerializer](../interfaces/codearts_plugin_.NotebookSerializer.md)

## Table of contents

### Constructors

- [constructor](codearts_plugin_.NotebookData.md#constructor)

### Properties

- [cells](codearts_plugin_.NotebookData.md#cells)
- [metadata](codearts_plugin_.NotebookData.md#metadata)

## Constructors

### constructor

• **new NotebookData**(`cells`)

Create new notebook data.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cells` | [`NotebookCellData`](codearts_plugin_.NotebookCellData.md)[] | An array of cell data. |

#### Defined in

[index.d.ts:14135](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14135)

## Properties

### cells

• **cells**: [`NotebookCellData`](codearts_plugin_.NotebookCellData.md)[]

The cell data of this notebook data.

#### Defined in

[index.d.ts:14123](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14123)

___

### metadata

• `Optional` **metadata**: `Object`

Arbitrary metadata of notebook data.

#### Index signature

▪ [key: `string`]: `any`

#### Defined in

[index.d.ts:14128](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14128)
