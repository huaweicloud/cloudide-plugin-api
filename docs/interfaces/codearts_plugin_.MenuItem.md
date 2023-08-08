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

[index.d.ts:17917](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17917)

___

### command

• **command**: [`CommandAction`](codearts_plugin_.CommandAction.md)

Command action.

#### Defined in

[index.d.ts:17897](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17897)

___

### group

• `Optional` **group**: `string`

Menu show in group.

#### Defined in

[index.d.ts:17907](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17907)

___

### order

• `Optional` **order**: `number`

The menu shown order.

#### Defined in

[index.d.ts:17912](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17912)

___

### when

• `Optional` **when**: `string`

ContextKey Expression.

#### Defined in

[index.d.ts:17902](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17902)
