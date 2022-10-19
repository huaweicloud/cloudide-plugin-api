[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DataTransfer

# Class: DataTransfer

["@codearts/plugin"](../modules/_codearts_plugin_.md).DataTransfer

A map containing a mapping of the mime type of the corresponding transferred data.

Drag and drop controllers that implement [`handleDrag`](../interfaces/codearts_plugin_.TreeDragAndDropController.md#handledrag) can add additional mime types to the
data transfer. These additional mime types will only be included in the `handleDrop` when the the drag was initiated from
an element in the same drag and drop controller.

## Implements

- `Iterable`<[mimeType: string, item: DataTransferItem]\>

## Table of contents

### Constructors

- [constructor](codearts_plugin_.DataTransfer.md#constructor)

### Methods

- [[iterator]](codearts_plugin_.DataTransfer.md#[iterator])
- [forEach](codearts_plugin_.DataTransfer.md#foreach)
- [get](codearts_plugin_.DataTransfer.md#get)
- [set](codearts_plugin_.DataTransfer.md#set)

## Constructors

### constructor

• **new DataTransfer**()

## Methods

### [iterator]

▸ **[iterator]**(): `IterableIterator`<[mimeType: string, item: DataTransferItem]\>

Get a new iterator with the `[mime, item]` pairs for each element in this data transfer.

#### Returns

`IterableIterator`<[mimeType: string, item: DataTransferItem]\>

#### Implementation of

Iterable.\_\_@iterator@10

#### Defined in

[index.d.ts:10353](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L10353)

___

### forEach

▸ **forEach**(`callbackfn`, `thisArg?`): `void`

Allows iteration through the data transfer items.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callbackfn` | (`value`: [`DataTransferItem`](codearts_plugin_.DataTransferItem.md), `key`: `string`, `dataTransfer`: [`DataTransfer`](codearts_plugin_.DataTransfer.md)) => `void` | Callback for iteration through the data transfer items. |
| `thisArg?` | `any` | The `this` context used when invoking the handler function. |

#### Returns

`void`

#### Defined in

[index.d.ts:10348](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L10348)

___

### get

▸ **get**(`mimeType`): `undefined` \| [`DataTransferItem`](codearts_plugin_.DataTransferItem.md)

Retrieves the data transfer item for a given mime type.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mimeType` | `string` | The mime type to get the data transfer item for, such as `text/plain` or `image/png`.  Special mime types: - `text/uri-list` — A string with `toString()`ed Uris separated by `\r\n`. To specify a cursor position in the file, set the Uri's fragment to `L3,5`, where 3 is the line number and 5 is the column number. |

#### Returns

`undefined` \| [`DataTransferItem`](codearts_plugin_.DataTransferItem.md)

#### Defined in

[index.d.ts:10333](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L10333)

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

[index.d.ts:10340](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L10340)
