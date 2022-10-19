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

[index.d.ts:16547](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16547)

___

### command

• **command**: [`CommandAction`](codearts_plugin_.CommandAction.md)

Command action.

#### Defined in

[index.d.ts:16527](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16527)

___

### group

• `Optional` **group**: `string`

Menu show in group.

#### Defined in

[index.d.ts:16537](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16537)

___

### order

• `Optional` **order**: `number`

The menu shown order.

#### Defined in

[index.d.ts:16542](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16542)

___

### when

• `Optional` **when**: `string`

ContextKey Expression.

#### Defined in

[index.d.ts:16532](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16532)
