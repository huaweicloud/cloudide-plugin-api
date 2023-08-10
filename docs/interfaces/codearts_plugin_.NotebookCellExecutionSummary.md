[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookCellExecutionSummary

# Interface: NotebookCellExecutionSummary

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookCellExecutionSummary

The summary of a notebook cell execution.

## Table of contents

### Properties

- [executionOrder](codearts_plugin_.NotebookCellExecutionSummary.md#executionorder)
- [success](codearts_plugin_.NotebookCellExecutionSummary.md#success)
- [timing](codearts_plugin_.NotebookCellExecutionSummary.md#timing)

## Properties

### executionOrder

• `Optional` `Readonly` **executionOrder**: `number`

The order in which the execution happened.

#### Defined in

[index.d.ts:14079](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14079)

___

### success

• `Optional` `Readonly` **success**: `boolean`

If the execution finished successfully.

#### Defined in

[index.d.ts:14084](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14084)

___

### timing

• `Optional` `Readonly` **timing**: `Object`

The times at which execution started and ended, as unix timestamps

#### Type declaration

| Name | Type |
| :------ | :------ |
| `endTime` | `number` |
| `startTime` | `number` |

#### Defined in

[index.d.ts:14089](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14089)
