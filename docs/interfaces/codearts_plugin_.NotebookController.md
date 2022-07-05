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

[index.d.ts:13457](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L13457)

___

### detail

• `Optional` **detail**: `string`

#### Defined in

[index.d.ts:13462](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L13462)

___

### id

• `Readonly` **id**: `string`

#### Defined in

[index.d.ts:13425](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L13425)

___

### label

• **label**: `string`

#### Defined in

[index.d.ts:13452](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L13452)

___

### notebookType

• `Readonly` **notebookType**: `string`

#### Defined in

[index.d.ts:13430](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L13430)

___

### onDidChangeSelectedNotebooks

• `Readonly` **onDidChangeSelectedNotebooks**: [`Event`](codearts_plugin_.Event.md)<{ `notebook`: [`NotebookDocument`](codearts_plugin_.NotebookDocument.md) ; `selected`: `boolean`  }\>

#### Defined in

[index.d.ts:13515](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L13515)

___

### supportedLanguages

• `Optional` **supportedLanguages**: `string`[]

#### Defined in

[index.d.ts:13447](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L13447)

___

### supportsExecutionOrder

• `Optional` **supportsExecutionOrder**: `boolean`

#### Defined in

[index.d.ts:13468](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L13468)

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

[index.d.ts:13483](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L13483)

___

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:13529](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L13529)

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

[index.d.ts:13489](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L13489)

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

[index.d.ts:13503](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L13503)

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

[index.d.ts:13524](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L13524)
