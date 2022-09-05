[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DataTransferItem

# Class: DataTransferItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).DataTransferItem

A class for encapsulating data transferred during a drag and drop event.

You can use the `value` of the `DataTransferItem` to get back the object you put into it
so long as the extension that created the `DataTransferItem` runs in the same extension host.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.DataTransferItem.md#constructor)

### Properties

- [value](codearts_plugin_.DataTransferItem.md#value)

### Methods

- [asString](codearts_plugin_.DataTransferItem.md#asstring)

## Constructors

### constructor

• **new DataTransferItem**(`value`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `any` |

#### Defined in

[index.d.ts:10169](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10169)

## Properties

### value

• `Readonly` **value**: `any`

#### Defined in

[index.d.ts:10168](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10168)

## Methods

### asString

▸ **asString**(): [`Thenable`](../interfaces/Thenable.md)<`string`\>

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`string`\>

#### Defined in

[index.d.ts:10167](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10167)
