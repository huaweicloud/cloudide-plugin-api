[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / QuickPickItem

# Interface: QuickPickItem

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).QuickPickItem

Represents an item that can be selected from a list of items.

## Table of contents

### Properties

- [alwaysShow](cloudide_plugin_.QuickPickItem.md#alwaysshow)
- [description](cloudide_plugin_.QuickPickItem.md#description)
- [detail](cloudide_plugin_.QuickPickItem.md#detail)
- [label](cloudide_plugin_.QuickPickItem.md#label)
- [picked](cloudide_plugin_.QuickPickItem.md#picked)
- [type](cloudide_plugin_.QuickPickItem.md#type)

## Properties

### alwaysShow

• `Optional` **alwaysShow**: `boolean`

Always show this item.

#### Defined in

[index.d.ts:2178](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2178)

___

### description

• `Optional` **description**: `string`

The item description

#### Defined in

[index.d.ts:2163](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2163)

___

### detail

• `Optional` **detail**: `string`

The item detail

#### Defined in

[index.d.ts:2168](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2168)

___

### label

• **label**: `string`

The item label

#### Defined in

[index.d.ts:2158](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2158)

___

### picked

• `Optional` **picked**: `boolean`

Used for [QuickPickOptions.canPickMany](#QuickPickOptions.canPickMany)
not implemented yet

#### Defined in

[index.d.ts:2174](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2174)

___

### type

• `Optional` **type**: ``"item"`` \| ``"separator"``

#### Defined in

[index.d.ts:2154](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2154)
