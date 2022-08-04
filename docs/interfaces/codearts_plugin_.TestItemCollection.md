[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TestItemCollection

# Interface: TestItemCollection

["@codearts/plugin"](../modules/_codearts_plugin_.md).TestItemCollection

## Table of contents

### Properties

- [size](codearts_plugin_.TestItemCollection.md#size)

### Methods

- [add](codearts_plugin_.TestItemCollection.md#add)
- [delete](codearts_plugin_.TestItemCollection.md#delete)
- [forEach](codearts_plugin_.TestItemCollection.md#foreach)
- [get](codearts_plugin_.TestItemCollection.md#get)
- [replace](codearts_plugin_.TestItemCollection.md#replace)

## Properties

### size

• `Readonly` **size**: `number`

#### Defined in

[index.d.ts:15675](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15675)

## Methods

### add

▸ **add**(`item`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`TestItem`](codearts_plugin_.TestItem.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:15696](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15696)

___

### delete

▸ **delete**(`itemId`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `itemId` | `string` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:15702](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15702)

___

### forEach

▸ **forEach**(`callback`, `thisArg?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`item`: [`TestItem`](codearts_plugin_.TestItem.md), `collection`: [`TestItemCollection`](codearts_plugin_.TestItemCollection.md)) => `unknown` |  |
| `thisArg?` | `unknown` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:15689](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15689)

___

### get

▸ **get**(`itemId`): `undefined` \| [`TestItem`](codearts_plugin_.TestItem.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `itemId` | `string` |  |

#### Returns

`undefined` \| [`TestItem`](codearts_plugin_.TestItem.md)

#### Defined in

[index.d.ts:15709](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15709)

___

### replace

▸ **replace**(`items`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | readonly [`TestItem`](codearts_plugin_.TestItem.md)[] |  |

#### Returns

`void`

#### Defined in

[index.d.ts:15681](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15681)
