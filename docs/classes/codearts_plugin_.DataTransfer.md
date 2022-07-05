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

[index.d.ts:10110](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L10110)

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

[index.d.ts:10097](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L10097)

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

[index.d.ts:10104](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L10104)
