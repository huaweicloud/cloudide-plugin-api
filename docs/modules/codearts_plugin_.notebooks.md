[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / notebooks

# Namespace: notebooks

["@codearts/plugin"](_codearts_plugin_.md).notebooks

Namespace for notebooks.

The notebooks functionality is composed of three loosely coupled components:

1. [NotebookSerializer](../interfaces/codearts_plugin_.NotebookSerializer.md) enable the editor to open, show, and save notebooks
2. [NotebookController](../interfaces/codearts_plugin_.NotebookController.md) own the execution of notebooks, e.g they create output from code cells.
3. NotebookRenderer present notebook output in the editor. They run in a separate context.

## Table of contents

### Functions

- [createNotebookController](codearts_plugin_.notebooks.md#createnotebookcontroller)
- [createRendererMessaging](codearts_plugin_.notebooks.md#createrenderermessaging)
- [registerNotebookCellStatusBarItemProvider](codearts_plugin_.notebooks.md#registernotebookcellstatusbaritemprovider)

## Functions

### createNotebookController

▸ **createNotebookController**(`id`, `notebookType`, `label`, `handler?`): [`NotebookController`](../interfaces/codearts_plugin_.NotebookController.md)

Creates a new notebook controller.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | Identifier of the controller. Must be unique per extension. |
| `notebookType` | `string` | A notebook type for which this controller is for. |
| `label` | `string` | The label of the controller. |
| `handler?` | (`cells`: [`NotebookCell`](../interfaces/codearts_plugin_.NotebookCell.md)[], `notebook`: [`NotebookDocument`](../interfaces/codearts_plugin_.NotebookDocument.md), `controller`: [`NotebookController`](../interfaces/codearts_plugin_.NotebookController.md)) => `void` \| [`Thenable`](../interfaces/Thenable.md)<`void`\> | The execute-handler of the controller. |

#### Returns

[`NotebookController`](../interfaces/codearts_plugin_.NotebookController.md)

#### Defined in

[index.d.ts:13819](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13819)

___

### createRendererMessaging

▸ **createRendererMessaging**(`rendererId`): [`NotebookRendererMessaging`](../interfaces/codearts_plugin_.NotebookRendererMessaging.md)

Creates a new messaging instance used to communicate with a specific renderer.

* *Note 1:* Extensions can only create renderer that they have defined in their `package.json`-file
* *Note 2:* A renderer only has access to messaging if `requiresMessaging` is set to `always` or `optional` in
its `notebookRenderer` contribution.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rendererId` | `string` | The renderer ID to communicate with |

#### Returns

[`NotebookRendererMessaging`](../interfaces/codearts_plugin_.NotebookRendererMessaging.md)

A new notebook renderer messaging object.

#### Defined in

[index.d.ts:13840](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13840)

___

### registerNotebookCellStatusBarItemProvider

▸ **registerNotebookCellStatusBarItemProvider**(`notebookType`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a [cell statusbar item provider](../interfaces/codearts_plugin_.NotebookCellStatusBarItemProvider.md) for the given notebook type.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `notebookType` | `string` | The notebook type to register for. |
| `provider` | [`NotebookCellStatusBarItemProvider`](../interfaces/codearts_plugin_.NotebookCellStatusBarItemProvider.md) | A cell status bar provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13828](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13828)
