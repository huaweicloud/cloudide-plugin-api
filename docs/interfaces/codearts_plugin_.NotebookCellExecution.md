[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookCellExecution

# Interface: NotebookCellExecution

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookCellExecution

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

#### Defined in

[index.d.ts:13545](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13545)

___

### executionOrder

• **executionOrder**: `undefined` \| `number`

#### Defined in

[index.d.ts:13559](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13559)

___

### token

• `Readonly` **token**: [`CancellationToken`](codearts_plugin_.CancellationToken.md)

#### Defined in

[index.d.ts:13554](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13554)

## Methods

### appendOutput

▸ **appendOutput**(`out`, `cell?`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `out` | [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md) \| readonly [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md)[] |  |
| `cell?` | [`NotebookCell`](codearts_plugin_.NotebookCell.md) |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:13606](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13606)

___

### appendOutputItems

▸ **appendOutputItems**(`items`, `output`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | [`NotebookCellOutputItem`](../classes/codearts_plugin_.NotebookCellOutputItem.md) \| readonly [`NotebookCellOutputItem`](../classes/codearts_plugin_.NotebookCellOutputItem.md)[] |  |
| `output` | [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md) |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:13624](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13624)

___

### clearOutput

▸ **clearOutput**(`cell?`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cell?` | [`NotebookCell`](codearts_plugin_.NotebookCell.md) |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:13586](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13586)

___

### end

▸ **end**(`success`, `endTime?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `success` | `undefined` \| `boolean` |  |
| `endTime?` | `number` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:13577](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13577)

___

### replaceOutput

▸ **replaceOutput**(`out`, `cell?`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `out` | [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md) \| readonly [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md)[] |  |
| `cell?` | [`NotebookCell`](codearts_plugin_.NotebookCell.md) |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:13596](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13596)

___

### replaceOutputItems

▸ **replaceOutputItems**(`items`, `output`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | [`NotebookCellOutputItem`](../classes/codearts_plugin_.NotebookCellOutputItem.md) \| readonly [`NotebookCellOutputItem`](../classes/codearts_plugin_.NotebookCellOutputItem.md)[] |  |
| `output` | [`NotebookCellOutput`](../classes/codearts_plugin_.NotebookCellOutput.md) |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:13615](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13615)

___

### start

▸ **start**(`startTime?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startTime?` | `number` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:13567](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L13567)
