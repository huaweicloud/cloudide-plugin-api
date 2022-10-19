[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookSerializer

# Interface: NotebookSerializer

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookSerializer

The notebook serializer enables the editor to open notebook files.

At its core the editor only knows a [notebook data structure](../classes/codearts_plugin_.NotebookData.md) but not
how that data structure is written to a file, nor how it is read from a file. The
notebook serializer bridges this gap by deserializing bytes into notebook data and
vice versa.

## Table of contents

### Methods

- [deserializeNotebook](codearts_plugin_.NotebookSerializer.md#deserializenotebook)
- [serializeNotebook](codearts_plugin_.NotebookSerializer.md#serializenotebook)

## Methods

### deserializeNotebook

▸ **deserializeNotebook**(`content`, `token`): [`NotebookData`](../classes/codearts_plugin_.NotebookData.md) \| [`Thenable`](Thenable.md)<[`NotebookData`](../classes/codearts_plugin_.NotebookData.md)\>

Deserialize contents of a notebook file into the notebook data structure.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `content` | `Uint8Array` | Contents of a notebook file. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`NotebookData`](../classes/codearts_plugin_.NotebookData.md) \| [`Thenable`](Thenable.md)<[`NotebookData`](../classes/codearts_plugin_.NotebookData.md)\>

Notebook data or a thenable that resolves to such.

#### Defined in

[index.d.ts:13598](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13598)

___

### serializeNotebook

▸ **serializeNotebook**(`data`, `token`): `Uint8Array` \| [`Thenable`](Thenable.md)<`Uint8Array`\>

Serialize notebook data into file contents.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`NotebookData`](../classes/codearts_plugin_.NotebookData.md) | A notebook data structure. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

`Uint8Array` \| [`Thenable`](Thenable.md)<`Uint8Array`\>

An array of bytes or a thenable that resolves to such.

#### Defined in

[index.d.ts:13607](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L13607)
