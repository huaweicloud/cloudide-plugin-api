[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookDocumentChangeEvent

# Interface: NotebookDocumentChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookDocumentChangeEvent

An event describing a transactional [notebook](codearts_plugin_.NotebookDocument.md) change.

## Table of contents

### Properties

- [cellChanges](codearts_plugin_.NotebookDocumentChangeEvent.md#cellchanges)
- [contentChanges](codearts_plugin_.NotebookDocumentChangeEvent.md#contentchanges)
- [metadata](codearts_plugin_.NotebookDocumentChangeEvent.md#metadata)
- [notebook](codearts_plugin_.NotebookDocumentChangeEvent.md#notebook)

## Properties

### cellChanges

• `Readonly` **cellChanges**: readonly [`NotebookDocumentCellChange`](codearts_plugin_.NotebookDocumentCellChange.md)[]

An array of [cell changes](codearts_plugin_.NotebookDocumentCellChange.md).

#### Defined in

[index.d.ts:14068](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14068)

___

### contentChanges

• `Readonly` **contentChanges**: readonly [`NotebookDocumentContentChange`](codearts_plugin_.NotebookDocumentContentChange.md)[]

An array of content changes describing added or removed [cells](codearts_plugin_.NotebookCell.md).

#### Defined in

[index.d.ts:14063](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14063)

___

### metadata

• `Readonly` **metadata**: `undefined` \| { `[key: string]`: `any`;  }

The new metadata of the notebook or `undefined` when it did not change.

#### Defined in

[index.d.ts:14058](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14058)

___

### notebook

• `Readonly` **notebook**: [`NotebookDocument`](codearts_plugin_.NotebookDocument.md)

The affected notebook.

#### Defined in

[index.d.ts:14053](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14053)
