[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookCellData

# Class: NotebookCellData

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookCellData

NotebookCellData is the raw representation of notebook cells. Its is part of [`NotebookData`](codearts_plugin_.NotebookData.md).

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

Create new cell data. Minimal cell data specifies its kind, its source value, and the
language identifier of its source.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | [`NotebookCellKind`](../enums/codearts_plugin_.NotebookCellKind.md) | The kind. |
| `value` | `string` | The source value. |
| `languageId` | `string` | The language identifier of the source value. |

#### Defined in

[index.d.ts:13722](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L13722)

## Properties

### executionSummary

• `Optional` **executionSummary**: [`NotebookCellExecutionSummary`](../interfaces/codearts_plugin_.NotebookCellExecutionSummary.md)

The execution summary of this cell data.

#### Defined in

[index.d.ts:13712](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L13712)

___

### kind

• **kind**: [`NotebookCellKind`](../enums/codearts_plugin_.NotebookCellKind.md)

The [kind](../enums/codearts_plugin_.NotebookCellKind.md) of this cell data.

#### Defined in

[index.d.ts:13686](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L13686)

___

### languageId

• **languageId**: `string`

The language identifier of the source value of this cell data. Any value from
[`getLanguages`](../modules/codearts_plugin_.languages.md#getlanguages) is possible.

#### Defined in

[index.d.ts:13697](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L13697)

___

### metadata

• `Optional` **metadata**: `Object`

Arbitrary metadata of this cell data. Can be anything but must be JSON-stringifyable.

#### Index signature

▪ [key: `string`]: `any`

#### Defined in

[index.d.ts:13707](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L13707)

___

### outputs

• `Optional` **outputs**: [`NotebookCellOutput`](codearts_plugin_.NotebookCellOutput.md)[]

The outputs of this cell data.

#### Defined in

[index.d.ts:13702](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L13702)

___

### value

• **value**: `string`

The source value of this cell data - either source code or formatted text.

#### Defined in

[index.d.ts:13691](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L13691)
