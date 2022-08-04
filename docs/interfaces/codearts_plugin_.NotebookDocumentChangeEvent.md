[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookDocumentChangeEvent

# Interface: NotebookDocumentChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookDocumentChangeEvent

## Table of contents

### Properties

- [cellChanges](codearts_plugin_.NotebookDocumentChangeEvent.md#cellchanges)
- [contentChanges](codearts_plugin_.NotebookDocumentChangeEvent.md#contentchanges)
- [metadata](codearts_plugin_.NotebookDocumentChangeEvent.md#metadata)
- [notebook](codearts_plugin_.NotebookDocumentChangeEvent.md#notebook)

## Properties

### cellChanges

• `Readonly` **cellChanges**: readonly [`NotebookDocumentCellChange`](codearts_plugin_.NotebookDocumentCellChange.md)[]

#### Defined in

[index.d.ts:13104](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13104)

___

### contentChanges

• `Readonly` **contentChanges**: readonly [`NotebookDocumentContentChange`](codearts_plugin_.NotebookDocumentContentChange.md)[]

#### Defined in

[index.d.ts:13099](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13099)

___

### metadata

• `Readonly` **metadata**: `undefined` \| { `[key: string]`: `any`;  }

#### Defined in

[index.d.ts:13094](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13094)

___

### notebook

• `Readonly` **notebook**: [`NotebookDocument`](codearts_plugin_.NotebookDocument.md)

#### Defined in

[index.d.ts:13089](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13089)
