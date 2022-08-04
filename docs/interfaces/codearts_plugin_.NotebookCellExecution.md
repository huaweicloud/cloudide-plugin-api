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

[index.d.ts:13575](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13575)

___

### executionOrder

• **executionOrder**: `undefined` \| `number`

#### Defined in

[index.d.ts:13589](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13589)

___

### token

• `Readonly` **token**: [`CancellationToken`](codearts_plugin_.CancellationToken.md)

#### Defined in

[index.d.ts:13584](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13584)

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

[index.d.ts:13636](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13636)

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

[index.d.ts:13654](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13654)

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

[index.d.ts:13616](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13616)

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

[index.d.ts:13607](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13607)

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

[index.d.ts:13626](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13626)

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

[index.d.ts:13645](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13645)

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

[index.d.ts:13597](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13597)
