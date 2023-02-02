[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / MenuItem

# Interface: MenuItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).MenuItem

## Table of contents

### Properties

- [args](codearts_plugin_.MenuItem.md#args)
- [command](codearts_plugin_.MenuItem.md#command)
- [group](codearts_plugin_.MenuItem.md#group)
- [order](codearts_plugin_.MenuItem.md#order)
- [when](codearts_plugin_.MenuItem.md#when)

## Properties

### args

• `Optional` **args**: `any`

Arguments passed to command, will be spreaded as rest parameters if this is an array

#### Defined in

[index.d.ts:16935](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16935)

___

### command

• **command**: [`CommandAction`](codearts_plugin_.CommandAction.md)

Command action.

#### Defined in

[index.d.ts:16915](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16915)

___

### group

• `Optional` **group**: `string`

Menu show in group.

#### Defined in

[index.d.ts:16925](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16925)

___

### order

• `Optional` **order**: `number`

The menu shown order.

#### Defined in

[index.d.ts:16930](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16930)

___

### when

• `Optional` **when**: `string`

ContextKey Expression.

#### Defined in

[index.d.ts:16920](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16920)
