[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookCell

# Interface: NotebookCell

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookCell

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

#### Defined in

[index.d.ts:12892](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L12892)

___

### executionSummary

• `Readonly` **executionSummary**: `undefined` \| [`NotebookCellExecutionSummary`](codearts_plugin_.NotebookCellExecutionSummary.md)

#### Defined in

[index.d.ts:12907](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L12907)

___

### index

• `Readonly` **index**: `number`

#### Defined in

[index.d.ts:12877](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L12877)

___

### kind

• `Readonly` **kind**: [`NotebookCellKind`](../enums/codearts_plugin_.NotebookCellKind.md)

#### Defined in

[index.d.ts:12887](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L12887)

___

### metadata

• `Readonly` **metadata**: `Object`

#### Index signature

▪ [key: `string`]: `any`

#### Defined in

[index.d.ts:12897](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L12897)

___

### notebook

• `Readonly` **notebook**: [`NotebookDocument`](codearts_plugin_.NotebookDocument.md)

#### Defined in

[index.d.ts:12882](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L12882)

___

### outputs

• `Readonly` **outputs**: readonly [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md)[]

#### Defined in

[index.d.ts:12902](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L12902)
