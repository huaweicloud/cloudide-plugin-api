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

[index.d.ts:15645](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L15645)

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

[index.d.ts:15666](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L15666)

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

[index.d.ts:15672](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L15672)

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

[index.d.ts:15659](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L15659)

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

[index.d.ts:15679](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L15679)

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

[index.d.ts:15651](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L15651)
