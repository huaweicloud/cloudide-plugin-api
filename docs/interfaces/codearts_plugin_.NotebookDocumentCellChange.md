[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookDocumentCellChange

# Interface: NotebookDocumentCellChange

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookDocumentCellChange

Describes a change to a notebook cell.

**`See`**

[NotebookDocumentChangeEvent](codearts_plugin_.NotebookDocumentChangeEvent.md)

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

The affected notebook.

#### Defined in

[index.d.ts:13861](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L13861)

___

### document

• `Readonly` **document**: `undefined` \| [`TextDocument`](codearts_plugin_.TextDocument.md)

The document of the cell or `undefined` when it did not change.

*Note* that you should use the [onDidChangeTextDocument](../modules/codearts_plugin_.workspace.md#ondidchangetextdocument)-event
for detailed change information, like what edits have been performed.

#### Defined in

[index.d.ts:13869](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L13869)

___

### executionSummary

• `Readonly` **executionSummary**: `undefined` \| [`NotebookCellExecutionSummary`](codearts_plugin_.NotebookCellExecutionSummary.md)

The new execution summary of the cell or `undefined` when it did not change.

#### Defined in

[index.d.ts:13884](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L13884)

___

### metadata

• `Readonly` **metadata**: `undefined` \| { `[key: string]`: `any`;  }

The new metadata of the cell or `undefined` when it did not change.

#### Defined in

[index.d.ts:13874](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L13874)

___

### outputs

• `Readonly` **outputs**: `undefined` \| readonly [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md)[]

The new outputs of the cell or `undefined` when they did not change.

#### Defined in

[index.d.ts:13879](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L13879)
