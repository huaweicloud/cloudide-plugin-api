[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookCellData

# Class: NotebookCellData

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookCellData

## Table of contents

### Constructors

- [constructor](codearts_plugin_.NotebookCellData.md#constructor)

### Properties

- [executionSummary](codearts_plugin_.NotebookCellData.md#executionsummary)
- [kind](codearts_plugin_.NotebookCellData.md#kind)
- [languageId](codearts_plugin_.NotebookCellData.md#languageid)
- [metadata](codearts_plugin_.NotebookCellData.md#metadata)
- [outputs](codearts_plugin_.NotebookCellData.md#outputs)
- [value](codearts_plugin_.NotebookCellData.md#value)

## Constructors

### constructor

• **new NotebookCellData**(`kind`, `value`, `languageId`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | [`NotebookCellKind`](../enums/codearts_plugin_.NotebookCellKind.md) |  |
| `value` | `string` |  |
| `languageId` | `string` |  |

#### Defined in

[index.d.ts:13328](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13328)

## Properties

### executionSummary

• `Optional` **executionSummary**: [`NotebookCellExecutionSummary`](../interfaces/codearts_plugin_.NotebookCellExecutionSummary.md)

#### Defined in

[index.d.ts:13318](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13318)

___

### kind

• **kind**: [`NotebookCellKind`](../enums/codearts_plugin_.NotebookCellKind.md)

#### Defined in

[index.d.ts:13292](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13292)

___

### languageId

• **languageId**: `string`

#### Defined in

[index.d.ts:13303](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13303)

___

### metadata

• `Optional` **metadata**: `Object`

#### Index signature

▪ [key: `string`]: `any`

#### Defined in

[index.d.ts:13313](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13313)

___

### outputs

• `Optional` **outputs**: [`NotebookCellOutput`](codearts_plugin_.NotebookCellOutput.md)[]

#### Defined in

[index.d.ts:13308](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13308)

___

### value

• **value**: `string`

#### Defined in

[index.d.ts:13297](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13297)
