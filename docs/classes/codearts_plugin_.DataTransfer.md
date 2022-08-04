[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DataTransfer

# Class: DataTransfer

["@codearts/plugin"](../modules/_codearts_plugin_.md).DataTransfer

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callbackfn` | (`value`: [`DataTransferItem`](codearts_plugin_.DataTransferItem.md), `key`: `string`) => `void` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:10140](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10140)

___

### get

▸ **get**(`mimeType`): `undefined` \| [`DataTransferItem`](codearts_plugin_.DataTransferItem.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mimeType` | `string` |  |

#### Returns

`undefined` \| [`DataTransferItem`](codearts_plugin_.DataTransferItem.md)

#### Defined in

[index.d.ts:10127](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10127)

___

### set

▸ **set**(`mimeType`, `value`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mimeType` | `string` |  |
| `value` | [`DataTransferItem`](codearts_plugin_.DataTransferItem.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:10134](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10134)
