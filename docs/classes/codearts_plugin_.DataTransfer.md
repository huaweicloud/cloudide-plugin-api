[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DataTransfer

# Class: DataTransfer

["@codearts/plugin"](../modules/_codearts_plugin_.md).DataTransfer

A map containing a mapping of the mime type of the corresponding transferred data.

Drag and drop controllers that implement [`handleDrag`](../interfaces/codearts_plugin_.TreeDragAndDropController.md#handledrag) can add additional mime types to the
data transfer. These additional mime types will only be included in the `handleDrop` when the the drag was initiated from
an element in the same drag and drop controller.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.DataTransfer.md#constructor)

### Methods

- [forEach](codearts_plugin_.DataTransfer.md#foreach)
- [get](codearts_plugin_.DataTransfer.md#get)
- [set](codearts_plugin_.DataTransfer.md#set)

## Constructors

### constructor

• **new DataTransfer**()

## Methods

### forEach

▸ **forEach**(`callbackfn`): `void`

Allows iteration through the data transfer items.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callbackfn` | (`value`: [`DataTransferItem`](codearts_plugin_.DataTransferItem.md), `key`: `string`) => `void` | Callback for iteration through the data transfer items. |

#### Returns

`void`

#### Defined in

[index.d.ts:10202](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10202)

___

### get

▸ **get**(`mimeType`): `undefined` \| [`DataTransferItem`](codearts_plugin_.DataTransferItem.md)

Retrieves the data transfer item for a given mime type.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mimeType` | `string` | The mime type to get the data transfer item for, such as `text/plain` or `image/png`.  Special mime types: - `text/uri-list` — A string with `toString()`ed Uris separated by newlines. To specify a cursor position in the file, set the Uri's fragment to `L3,5`, where 3 is the line number and 5 is the column number. |

#### Returns

`undefined` \| [`DataTransferItem`](codearts_plugin_.DataTransferItem.md)

#### Defined in

[index.d.ts:10189](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10189)

___

### set

▸ **set**(`mimeType`, `value`): `void`

Sets a mime type to data transfer item mapping.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mimeType` | `string` | The mime type to set the data for. |
| `value` | [`DataTransferItem`](codearts_plugin_.DataTransferItem.md) | The data transfer item for the given mime type. |

#### Returns

`void`

#### Defined in

[index.d.ts:10196](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10196)
