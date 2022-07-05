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

[index.d.ts:13298](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L13298)

## Properties

### executionSummary

• `Optional` **executionSummary**: [`NotebookCellExecutionSummary`](../interfaces/codearts_plugin_.NotebookCellExecutionSummary.md)

#### Defined in

[index.d.ts:13288](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L13288)

___

### kind

• **kind**: [`NotebookCellKind`](../enums/codearts_plugin_.NotebookCellKind.md)

#### Defined in

[index.d.ts:13262](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L13262)

___

### languageId

• **languageId**: `string`

#### Defined in

[index.d.ts:13273](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L13273)

___

### metadata

• `Optional` **metadata**: `Object`

#### Index signature

▪ [key: `string`]: `any`

#### Defined in

[index.d.ts:13283](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L13283)

___

### outputs

• `Optional` **outputs**: [`NotebookCellOutput`](codearts_plugin_.NotebookCellOutput.md)[]

#### Defined in

[index.d.ts:13278](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L13278)

___

### value

• **value**: `string`

#### Defined in

[index.d.ts:13267](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L13267)
