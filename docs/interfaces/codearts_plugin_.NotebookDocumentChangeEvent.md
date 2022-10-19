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

[index.d.ts:13327](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13327)

___

### contentChanges

• `Readonly` **contentChanges**: readonly [`NotebookDocumentContentChange`](codearts_plugin_.NotebookDocumentContentChange.md)[]

An array of content changes describing added or removed [cells](codearts_plugin_.NotebookCell.md).

#### Defined in

[index.d.ts:13322](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13322)

___

### metadata

• `Readonly` **metadata**: `undefined` \| { `[key: string]`: `any`;  }

The new metadata of the notebook or `undefined` when it did not change.

#### Defined in

[index.d.ts:13317](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13317)

___

### notebook

• `Readonly` **notebook**: [`NotebookDocument`](codearts_plugin_.NotebookDocument.md)

The affected notebook.

#### Defined in

[index.d.ts:13312](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13312)
