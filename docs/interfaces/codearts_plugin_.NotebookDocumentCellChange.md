[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookDocumentCellChange

# Interface: NotebookDocumentCellChange

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookDocumentCellChange

## Table of contents

### Properties

- [cell](codearts_plugin_.NotebookDocumentCellChange.md#cell)
- [document](codearts_plugin_.NotebookDocumentCellChange.md#document)
- [executionSummary](codearts_plugin_.NotebookDocumentCellChange.md#executionsummary)
- [metadata](codearts_plugin_.NotebookDocumentCellChange.md#metadata)
- [outputs](codearts_plugin_.NotebookDocumentCellChange.md#outputs)

## Properties

### cell

• `Readonly` **cell**: [`NotebookCell`](codearts_plugin_.NotebookCell.md)

#### Defined in

[index.d.ts:13029](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13029)

___

### document

• `Readonly` **document**: `undefined` \| [`TextDocument`](codearts_plugin_.TextDocument.md)

#### Defined in

[index.d.ts:13037](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13037)

___

### executionSummary

• `Readonly` **executionSummary**: `undefined` \| [`NotebookCellExecutionSummary`](codearts_plugin_.NotebookCellExecutionSummary.md)

#### Defined in

[index.d.ts:13052](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13052)

___

### metadata

• `Readonly` **metadata**: `undefined` \| { `[key: string]`: `any`;  }

#### Defined in

[index.d.ts:13042](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13042)

___

### outputs

• `Readonly` **outputs**: `undefined` \| readonly [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md)[]

#### Defined in

[index.d.ts:13047](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13047)
