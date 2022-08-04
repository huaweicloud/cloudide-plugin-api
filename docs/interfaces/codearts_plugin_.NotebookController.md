[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookController

# Interface: NotebookController

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookController

## Table of contents

### Properties

- [description](codearts_plugin_.NotebookController.md#description)
- [detail](codearts_plugin_.NotebookController.md#detail)
- [id](codearts_plugin_.NotebookController.md#id)
- [label](codearts_plugin_.NotebookController.md#label)
- [notebookType](codearts_plugin_.NotebookController.md#notebooktype)
- [onDidChangeSelectedNotebooks](codearts_plugin_.NotebookController.md#ondidchangeselectednotebooks)
- [supportedLanguages](codearts_plugin_.NotebookController.md#supportedlanguages)
- [supportsExecutionOrder](codearts_plugin_.NotebookController.md#supportsexecutionorder)

### Methods

- [createNotebookCellExecution](codearts_plugin_.NotebookController.md#createnotebookcellexecution)
- [dispose](codearts_plugin_.NotebookController.md#dispose)
- [executeHandler](codearts_plugin_.NotebookController.md#executehandler)
- [interruptHandler](codearts_plugin_.NotebookController.md#interrupthandler)
- [updateNotebookAffinity](codearts_plugin_.NotebookController.md#updatenotebookaffinity)

## Properties

### description

• `Optional` **description**: `string`

#### Defined in

[index.d.ts:13487](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13487)

___

### detail

• `Optional` **detail**: `string`

#### Defined in

[index.d.ts:13492](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13492)

___

### id

• `Readonly` **id**: `string`

#### Defined in

[index.d.ts:13455](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13455)

___

### label

• **label**: `string`

#### Defined in

[index.d.ts:13482](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13482)

___

### notebookType

• `Readonly` **notebookType**: `string`

#### Defined in

[index.d.ts:13460](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13460)

___

### onDidChangeSelectedNotebooks

• `Readonly` **onDidChangeSelectedNotebooks**: [`Event`](codearts_plugin_.Event.md)<{ `notebook`: [`NotebookDocument`](codearts_plugin_.NotebookDocument.md) ; `selected`: `boolean`  }\>

#### Defined in

[index.d.ts:13545](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13545)

___

### supportedLanguages

• `Optional` **supportedLanguages**: `string`[]

#### Defined in

[index.d.ts:13477](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13477)

___

### supportsExecutionOrder

• `Optional` **supportsExecutionOrder**: `boolean`

#### Defined in

[index.d.ts:13498](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13498)

## Methods

### createNotebookCellExecution

▸ **createNotebookCellExecution**(`cell`): [`NotebookCellExecution`](codearts_plugin_.NotebookCellExecution.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cell` | [`NotebookCell`](codearts_plugin_.NotebookCell.md) |  |

#### Returns

[`NotebookCellExecution`](codearts_plugin_.NotebookCellExecution.md)

#### Defined in

[index.d.ts:13513](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13513)

___

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:13559](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13559)

___

### executeHandler

▸ **executeHandler**(`cells`, `notebook`, `controller`): `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `cells` | [`NotebookCell`](codearts_plugin_.NotebookCell.md)[] |
| `notebook` | [`NotebookDocument`](codearts_plugin_.NotebookDocument.md) |
| `controller` | [`NotebookController`](codearts_plugin_.NotebookController.md) |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:13519](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13519)

___

### interruptHandler

▸ `Optional` **interruptHandler**(`notebook`): `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `notebook` | [`NotebookDocument`](codearts_plugin_.NotebookDocument.md) |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:13533](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13533)

___

### updateNotebookAffinity

▸ **updateNotebookAffinity**(`notebook`, `affinity`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `notebook` | [`NotebookDocument`](codearts_plugin_.NotebookDocument.md) |  |
| `affinity` | [`NotebookControllerAffinity`](../enums/codearts_plugin_.NotebookControllerAffinity.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:13554](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13554)
