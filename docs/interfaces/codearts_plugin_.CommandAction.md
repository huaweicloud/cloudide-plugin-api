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

[index.d.ts:17634](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17634)

___

### icon

• `Optional` **icon**: [`MenuThemeIcon`](codearts_plugin_.MenuThemeIcon.md)

Menu icon.

#### Defined in

[index.d.ts:17644](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17644)

___

### id

• **id**: `string`

Command id.

#### Defined in

[index.d.ts:17619](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17619)

___

### precondition

• `Optional` **precondition**: `string`

ContextKey Expression.

#### Defined in

[index.d.ts:17654](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17654)

___

### shortTitle

• `Optional` **shortTitle**: `string`

Short title show on menu.

#### Defined in

[index.d.ts:17629](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17629)

___

### source

• `Optional` **source**: `string`

Menu source.

#### Defined in

[index.d.ts:17649](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17649)

___

### title

• **title**: `string`

Title show on menu.

#### Defined in

[index.d.ts:17624](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17624)

___

### toggled

• `Optional` **toggled**: `string` \| { `condition`: `string` ; `icon?`: [`MenuThemeIcon`](codearts_plugin_.MenuThemeIcon.md) ; `title?`: `string` ; `tooltip?`: `string`  }

ContextKey Expression.

#### Defined in

[index.d.ts:17659](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17659)

___

### tooltip

• `Optional` **tooltip**: `string`

Tooltip title.

#### Defined in

[index.d.ts:17639](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L17639)
