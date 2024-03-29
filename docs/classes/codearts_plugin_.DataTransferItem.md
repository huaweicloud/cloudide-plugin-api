[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DataTransferItem

# Class: DataTransferItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).DataTransferItem

Encapsulates data transferred during drag and drop operations.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.DataTransferItem.md#constructor)

### Properties

- [value](codearts_plugin_.DataTransferItem.md#value)

### Methods

- [asFile](codearts_plugin_.DataTransferItem.md#asfile)
- [asString](codearts_plugin_.DataTransferItem.md#asstring)

## Constructors

### constructor

• **new DataTransferItem**(`value`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | Custom data stored on this item. Can be retrieved using [`value`](codearts_plugin_.DataTransferItem.md#value). |

#### Defined in

[index.d.ts:10638](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L10638)

## Properties

### value

• `Readonly` **value**: `any`

Custom data stored on this item.

You can use `value` to share data across operations. The original object can be retrieved so long as the extension that
created the `DataTransferItem` runs in the same extension host.

#### Defined in

[index.d.ts:10633](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L10633)

## Methods

### asFile

▸ **asFile**(): `undefined` \| [`DataTransferFile`](../interfaces/codearts_plugin_.DataTransferFile.md)

Try getting the [file](../interfaces/codearts_plugin_.DataTransferFile.md) associated with this data transfer item.

Note that the file object is only valid for the scope of the drag and drop operation.

#### Returns

`undefined` \| [`DataTransferFile`](../interfaces/codearts_plugin_.DataTransferFile.md)

The file for the data transfer or `undefined` if the item is either not a file or the
file data cannot be accessed.

#### Defined in

[index.d.ts:10625](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L10625)

___

### asString

▸ **asString**(): [`Thenable`](../interfaces/Thenable.md)<`string`\>

Get a string representation of this item.

If [`value`](codearts_plugin_.DataTransferItem.md#value) is an object, this returns the result of json stringifying [`value`](codearts_plugin_.DataTransferItem.md#value) value.

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`string`\>

#### Defined in

[index.d.ts:10615](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L10615)
