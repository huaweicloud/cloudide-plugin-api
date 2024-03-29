[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookCell

# Interface: NotebookCell

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookCell

Represents a cell of a [notebook](codearts_plugin_.NotebookDocument.md), either a [code](../enums/codearts_plugin_.NotebookCellKind.md#code)-cell
or [markup](../enums/codearts_plugin_.NotebookCellKind.md#markup)-cell.

NotebookCell instances are immutable and are kept in sync for as long as they are part of their notebook.

## Table of contents

### Properties

- [document](codearts_plugin_.NotebookCell.md#document)
- [executionSummary](codearts_plugin_.NotebookCell.md#executionsummary)
- [index](codearts_plugin_.NotebookCell.md#index)
- [kind](codearts_plugin_.NotebookCell.md#kind)
- [metadata](codearts_plugin_.NotebookCell.md#metadata)
- [notebook](codearts_plugin_.NotebookCell.md#notebook)
- [outputs](codearts_plugin_.NotebookCell.md#outputs)

## Properties

### document

• `Readonly` **document**: [`TextDocument`](codearts_plugin_.TextDocument.md)

The [text](codearts_plugin_.TextDocument.md) of this cell, represented as text document.

#### Defined in

[index.d.ts:13886](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13886)

___

### executionSummary

• `Readonly` **executionSummary**: `undefined` \| [`NotebookCellExecutionSummary`](codearts_plugin_.NotebookCellExecutionSummary.md)

The most recent [execution summary](codearts_plugin_.NotebookCellExecutionSummary.md) for this cell.

#### Defined in

[index.d.ts:13901](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13901)

___

### index

• `Readonly` **index**: `number`

The index of this cell in its [containing notebook](codearts_plugin_.NotebookDocument.md#cellat). The
index is updated when a cell is moved within its notebook. The index is `-1`
when the cell has been removed from its notebook.

#### Defined in

[index.d.ts:13871](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13871)

___

### kind

• `Readonly` **kind**: [`NotebookCellKind`](../enums/codearts_plugin_.NotebookCellKind.md)

The kind of this cell.

#### Defined in

[index.d.ts:13881](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13881)

___

### metadata

• `Readonly` **metadata**: `Object`

The metadata of this cell. Can be anything but must be JSON-stringifyable.

#### Index signature

▪ [key: `string`]: `any`

#### Defined in

[index.d.ts:13891](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13891)

___

### notebook

• `Readonly` **notebook**: [`NotebookDocument`](codearts_plugin_.NotebookDocument.md)

The [notebook](codearts_plugin_.NotebookDocument.md) that contains this cell.

#### Defined in

[index.d.ts:13876](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13876)

___

### outputs

• `Readonly` **outputs**: readonly [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md)[]

The outputs of this cell.

#### Defined in

[index.d.ts:13896](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13896)
