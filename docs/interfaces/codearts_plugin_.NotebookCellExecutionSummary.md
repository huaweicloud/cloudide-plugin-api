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

[index.d.ts:14050](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14050)

___

### success

• `Optional` `Readonly` **success**: `boolean`

If the execution finished successfully.

#### Defined in

[index.d.ts:14055](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14055)

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

[index.d.ts:14060](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14060)
