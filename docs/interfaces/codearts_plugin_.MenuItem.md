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

[index.d.ts:17687](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17687)

___

### command

• **command**: [`CommandAction`](codearts_plugin_.CommandAction.md)

Command action.

#### Defined in

[index.d.ts:17667](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17667)

___

### group

• `Optional` **group**: `string`

Menu show in group.

#### Defined in

[index.d.ts:17677](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17677)

___

### order

• `Optional` **order**: `number`

The menu shown order.

#### Defined in

[index.d.ts:17682](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17682)

___

### when

• `Optional` **when**: `string`

ContextKey Expression.

#### Defined in

[index.d.ts:17672](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17672)
