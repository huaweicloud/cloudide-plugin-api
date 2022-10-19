[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CommandAction

# Interface: CommandAction

["@codearts/plugin"](../modules/_codearts_plugin_.md).CommandAction

## Table of contents

### Properties

- [category](codearts_plugin_.CommandAction.md#category)
- [icon](codearts_plugin_.CommandAction.md#icon)
- [id](codearts_plugin_.CommandAction.md#id)
- [precondition](codearts_plugin_.CommandAction.md#precondition)
- [shortTitle](codearts_plugin_.CommandAction.md#shorttitle)
- [source](codearts_plugin_.CommandAction.md#source)
- [title](codearts_plugin_.CommandAction.md#title)
- [toggled](codearts_plugin_.CommandAction.md#toggled)
- [tooltip](codearts_plugin_.CommandAction.md#tooltip)

## Properties

### category

• `Optional` **category**: `string`

Menu category in submenu.

#### Defined in

[index.d.ts:16494](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16494)

___

### icon

• `Optional` **icon**: [`MenuThemeIcon`](codearts_plugin_.MenuThemeIcon.md)

Menu icon.

#### Defined in

[index.d.ts:16504](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16504)

___

### id

• **id**: `string`

Command id.

#### Defined in

[index.d.ts:16479](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16479)

___

### precondition

• `Optional` **precondition**: `string`

ContextKey Expression.

#### Defined in

[index.d.ts:16514](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16514)

___

### shortTitle

• `Optional` **shortTitle**: `string`

Short title show on menu.

#### Defined in

[index.d.ts:16489](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16489)

___

### source

• `Optional` **source**: `string`

Menu source.

#### Defined in

[index.d.ts:16509](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16509)

___

### title

• **title**: `string`

Title show on menu.

#### Defined in

[index.d.ts:16484](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16484)

___

### toggled

• `Optional` **toggled**: `string` \| { `condition`: `string` ; `icon?`: [`MenuThemeIcon`](codearts_plugin_.MenuThemeIcon.md) ; `title?`: `string` ; `tooltip?`: `string`  }

ContextKey Expression.

#### Defined in

[index.d.ts:16519](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16519)

___

### tooltip

• `Optional` **tooltip**: `string`

Tooltip title.

#### Defined in

[index.d.ts:16499](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L16499)
