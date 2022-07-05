[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / notebooks

# Namespace: notebooks

["@codearts/plugin"](_codearts_plugin_.md).notebooks

## Table of contents

### Functions

- [createNotebookController](codearts_plugin_.notebooks.md#createnotebookcontroller)
- [createRendererMessaging](codearts_plugin_.notebooks.md#createrenderermessaging)
- [registerNotebookCellStatusBarItemProvider](codearts_plugin_.notebooks.md#registernotebookcellstatusbaritemprovider)

## Functions

### createNotebookController

▸ **createNotebookController**(`id`, `notebookType`, `label`, `handler?`): [`NotebookController`](../interfaces/codearts_plugin_.NotebookController.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` |  |
| `notebookType` | `string` |  |
| `label` | `string` |  |
| `handler?` | (`cells`: [`NotebookCell`](../interfaces/codearts_plugin_.NotebookCell.md)[], `notebook`: [`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md), `controller`: [`NotebookController`](../interfaces/codearts_plugin_.NotebookController.md)) => `void` \| [`Thenable`](../interfaces/Thenable.md)<`void`\> |  |

#### Returns

[`NotebookController`](../interfaces/codearts_plugin_.NotebookController.md)

#### Defined in

[index.d.ts:13727](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L13727)

___

### createRendererMessaging

▸ **createRendererMessaging**(`rendererId`): [`NotebookRendererMessaging`](../interfaces/codearts_plugin_.NotebookRendererMessaging.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rendererId` | `string` |  |

#### Returns

[`NotebookRendererMessaging`](../interfaces/codearts_plugin_.NotebookRendererMessaging.md)

#### Defined in

[index.d.ts:13748](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L13748)

___

### registerNotebookCellStatusBarItemProvider

▸ **registerNotebookCellStatusBarItemProvider**(`notebookType`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `notebookType` | `string` |  |
| `provider` | [`NotebookCellStatusBarItemProvider`](../interfaces/codearts_plugin_.NotebookCellStatusBarItemProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:13736](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L13736)
