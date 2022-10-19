[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookCellExecution

# Interface: NotebookCellExecution

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookCellExecution

A NotebookCellExecution is how [notebook controller](codearts_plugin_.NotebookController.md) modify a notebook cell as
it is executing.

When a cell execution object is created, the cell enters the NotebookCellExecutionState.Pending Pending state.
When [`start(...)`](codearts_plugin_.NotebookCellExecution.md#start) is called on the execution task, it enters the NotebookCellExecutionState.Executing Executing state. When
[`end(...)`](codearts_plugin_.NotebookCellExecution.md#end) is called, it enters the NotebookCellExecutionState.Idle Idle state.

## Table of contents

### Properties

- [cell](codearts_plugin_.NotebookCellExecution.md#cell)
- [executionOrder](codearts_plugin_.NotebookCellExecution.md#executionorder)
- [token](codearts_plugin_.NotebookCellExecution.md#token)

### Methods

- [appendOutput](codearts_plugin_.NotebookCellExecution.md#appendoutput)
- [appendOutputItems](codearts_plugin_.NotebookCellExecution.md#appendoutputitems)
- [clearOutput](codearts_plugin_.NotebookCellExecution.md#clearoutput)
- [end](codearts_plugin_.NotebookCellExecution.md#end)
- [replaceOutput](codearts_plugin_.NotebookCellExecution.md#replaceoutput)
- [replaceOutputItems](codearts_plugin_.NotebookCellExecution.md#replaceoutputitems)
- [start](codearts_plugin_.NotebookCellExecution.md#start)

## Properties

### cell

• `Readonly` **cell**: [`NotebookCell`](codearts_plugin_.NotebookCell.md)

The [cell](codearts_plugin_.NotebookCell.md) for which this execution has been created.

#### Defined in

[index.d.ts:13798](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13798)

___

### executionOrder

• **executionOrder**: `undefined` \| `number`

Set and unset the order of this cell execution.

#### Defined in

[index.d.ts:13812](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13812)

___

### token

• `Readonly` **token**: [`CancellationToken`](codearts_plugin_.CancellationToken.md)

A cancellation token which will be triggered when the cell execution is canceled
from the UI.

_Note_ that the cancellation token will not be triggered when the [controller](codearts_plugin_.NotebookController.md)
that created this execution uses an [interrupt-handler](codearts_plugin_.NotebookController.md#interrupthandler).

#### Defined in

[index.d.ts:13807](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13807)

## Methods

### appendOutput

▸ **appendOutput**(`out`, `cell?`): [`Thenable`](Thenable.md)<`void`\>

Append to the output of the cell that is executing or to another cell that is affected by this execution.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `out` | [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md) \| readonly [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md)[] | Output that is appended to the current output. |
| `cell?` | [`NotebookCell`](codearts_plugin_.NotebookCell.md) | Cell for which output is cleared. Defaults to the [cell](codearts_plugin_.NotebookCellExecution.md#cell) of this execution. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

A thenable that resolves when the operation finished.

#### Defined in

[index.d.ts:13859](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13859)

___

### appendOutputItems

▸ **appendOutputItems**(`items`, `output`): [`Thenable`](Thenable.md)<`void`\>

Append output items to existing cell output.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | [`NotebookCellOutputItem`](../classes/codearts_plugin_.NotebookCellOutputItem.md) \| readonly [`NotebookCellOutputItem`](../classes/codearts_plugin_.NotebookCellOutputItem.md)[] | Output items that are append to existing output. |
| `output` | [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md) | Output object that already exists. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

A thenable that resolves when the operation finished.

#### Defined in

[index.d.ts:13877](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13877)

___

### clearOutput

▸ **clearOutput**(`cell?`): [`Thenable`](Thenable.md)<`void`\>

Clears the output of the cell that is executing or of another cell that is affected by this execution.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cell?` | [`NotebookCell`](codearts_plugin_.NotebookCell.md) | Cell for which output is cleared. Defaults to the [cell](codearts_plugin_.NotebookCellExecution.md#cell) of this execution. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

A thenable that resolves when the operation finished.

#### Defined in

[index.d.ts:13839](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13839)

___

### end

▸ **end**(`success`, `endTime?`): `void`

Signal that execution has ended.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `success` | `undefined` \| `boolean` | If true, a green check is shown on the cell status bar. If false, a red X is shown. If undefined, no check or X icon is shown. |
| `endTime?` | `number` | The time that execution finished, in milliseconds in the Unix epoch. |

#### Returns

`void`

#### Defined in

[index.d.ts:13830](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13830)

___

### replaceOutput

▸ **replaceOutput**(`out`, `cell?`): [`Thenable`](Thenable.md)<`void`\>

Replace the output of the cell that is executing or of another cell that is affected by this execution.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `out` | [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md) \| readonly [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md)[] | Output that replaces the current output. |
| `cell?` | [`NotebookCell`](codearts_plugin_.NotebookCell.md) | Cell for which output is cleared. Defaults to the [cell](codearts_plugin_.NotebookCellExecution.md#cell) of this execution. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

A thenable that resolves when the operation finished.

#### Defined in

[index.d.ts:13849](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13849)

___

### replaceOutputItems

▸ **replaceOutputItems**(`items`, `output`): [`Thenable`](Thenable.md)<`void`\>

Replace all output items of existing cell output.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | [`NotebookCellOutputItem`](../classes/codearts_plugin_.NotebookCellOutputItem.md) \| readonly [`NotebookCellOutputItem`](../classes/codearts_plugin_.NotebookCellOutputItem.md)[] | Output items that replace the items of existing output. |
| `output` | [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md) | Output object that already exists. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

A thenable that resolves when the operation finished.

#### Defined in

[index.d.ts:13868](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13868)

___

### start

▸ **start**(`startTime?`): `void`

Signal that the execution has begun.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startTime?` | `number` | The time that execution began, in milliseconds in the Unix epoch. Used to drive the clock that shows for how long a cell has been running. If not given, the clock won't be shown. |

#### Returns

`void`

#### Defined in

[index.d.ts:13820](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13820)
