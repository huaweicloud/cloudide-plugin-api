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

[index.d.ts:17792](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17792)

___

### command

• **command**: [`CommandAction`](codearts_plugin_.CommandAction.md)

Command action.

#### Defined in

[index.d.ts:17772](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17772)

___

### group

• `Optional` **group**: `string`

Menu show in group.

#### Defined in

[index.d.ts:17782](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17782)

___

### order

• `Optional` **order**: `number`

The menu shown order.

#### Defined in

[index.d.ts:17787](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17787)

___

### when

• `Optional` **when**: `string`

ContextKey Expression.

#### Defined in

[index.d.ts:17777](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17777)
