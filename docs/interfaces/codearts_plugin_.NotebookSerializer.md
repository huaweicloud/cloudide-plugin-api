[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookSerializer

# Interface: NotebookSerializer

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookSerializer

## Table of contents

### Methods

- [deserializeNotebook](codearts_plugin_.NotebookSerializer.md#deserializenotebook)
- [serializeNotebook](codearts_plugin_.NotebookSerializer.md#serializenotebook)

## Methods

### deserializeNotebook

▸ **deserializeNotebook**(`content`, `token`): [`NotebookData`](../classes/codearts_plugin_.NotebookData.md) \| [`Thenable`](Thenable.md)<[`NotebookData`](../classes/codearts_plugin_.NotebookData.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `content` | `Uint8Array` |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`NotebookData`](../classes/codearts_plugin_.NotebookData.md) \| [`Thenable`](Thenable.md)<[`NotebookData`](../classes/codearts_plugin_.NotebookData.md)\>

#### Defined in

[index.d.ts:13345](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L13345)

___

### serializeNotebook

▸ **serializeNotebook**(`data`, `token`): `Uint8Array` \| [`Thenable`](Thenable.md)<`Uint8Array`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`NotebookData`](../classes/codearts_plugin_.NotebookData.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

`Uint8Array` \| [`Thenable`](Thenable.md)<`Uint8Array`\>

#### Defined in

[index.d.ts:13354](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L13354)
