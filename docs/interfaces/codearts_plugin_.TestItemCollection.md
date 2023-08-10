[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TestItemCollection

# Interface: TestItemCollection

["@codearts/plugin"](../modules/_codearts_plugin_.md).TestItemCollection

Collection of test items, found in [children](codearts_plugin_.TestItem.md#children) and
[items](codearts_plugin_.TestController.md#items).

## Hierarchy

- `Iterable`<[id: string, testItem: TestItem]\>

  ↳ **`TestItemCollection`**

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

Gets the number of items in the collection.

#### Defined in

[index.d.ts:16665](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16665)

## Methods

### add

▸ **add**(`item`): `void`

Adds the test item to the children. If an item with the same ID already
exists, it'll be replaced.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`TestItem`](codearts_plugin_.TestItem.md) | Item to add. |

#### Returns

`void`

#### Defined in

[index.d.ts:16686](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16686)

___

### delete

▸ **delete**(`itemId`): `void`

Removes a single test item from the collection.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `itemId` | `string` | Item ID to delete. |

#### Returns

`void`

#### Defined in

[index.d.ts:16692](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16692)

___

### forEach

▸ **forEach**(`callback`, `thisArg?`): `void`

Iterate over each entry in this collection.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`item`: [`TestItem`](codearts_plugin_.TestItem.md), `collection`: [`TestItemCollection`](codearts_plugin_.TestItemCollection.md)) => `unknown` | Function to execute for each entry. |
| `thisArg?` | `any` | The `this` context used when invoking the handler function. |

#### Returns

`void`

#### Defined in

[index.d.ts:16679](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16679)

___

### get

▸ **get**(`itemId`): `undefined` \| [`TestItem`](codearts_plugin_.TestItem.md)

Efficiently gets a test item by ID, if it exists, in the children.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `itemId` | `string` | Item ID to get. |

#### Returns

`undefined` \| [`TestItem`](codearts_plugin_.TestItem.md)

The found item or undefined if it does not exist.

#### Defined in

[index.d.ts:16699](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16699)

___

### replace

▸ **replace**(`items`): `void`

Replaces the items stored by the collection.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items` | readonly [`TestItem`](codearts_plugin_.TestItem.md)[] | Items to store. |

#### Returns

`void`

#### Defined in

[index.d.ts:16671](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16671)
