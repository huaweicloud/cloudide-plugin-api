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

[index.d.ts:16882](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16882)

___

### icon

• `Optional` **icon**: [`MenuThemeIcon`](codearts_plugin_.MenuThemeIcon.md)

Menu icon.

#### Defined in

[index.d.ts:16892](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16892)

___

### id

• **id**: `string`

Command id.

#### Defined in

[index.d.ts:16867](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16867)

___

### precondition

• `Optional` **precondition**: `string`

ContextKey Expression.

#### Defined in

[index.d.ts:16902](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16902)

___

### shortTitle

• `Optional` **shortTitle**: `string`

Short title show on menu.

#### Defined in

[index.d.ts:16877](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16877)

___

### source

• `Optional` **source**: `string`

Menu source.

#### Defined in

[index.d.ts:16897](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16897)

___

### title

• **title**: `string`

Title show on menu.

#### Defined in

[index.d.ts:16872](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16872)

___

### toggled

• `Optional` **toggled**: `string` \| { `condition`: `string` ; `icon?`: [`MenuThemeIcon`](codearts_plugin_.MenuThemeIcon.md) ; `title?`: `string` ; `tooltip?`: `string`  }

ContextKey Expression.

#### Defined in

[index.d.ts:16907](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16907)

___

### tooltip

• `Optional` **tooltip**: `string`

Tooltip title.

#### Defined in

[index.d.ts:16887](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16887)
