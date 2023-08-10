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

[index.d.ts:17848](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17848)

___

### icon

• `Optional` **icon**: [`MenuThemeIcon`](codearts_plugin_.MenuThemeIcon.md)

Menu icon.

#### Defined in

[index.d.ts:17858](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17858)

___

### id

• **id**: `string`

Command id.

#### Defined in

[index.d.ts:17833](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17833)

___

### precondition

• `Optional` **precondition**: `string`

ContextKey Expression.

#### Defined in

[index.d.ts:17868](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17868)

___

### shortTitle

• `Optional` **shortTitle**: `string`

Short title show on menu.

#### Defined in

[index.d.ts:17843](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17843)

___

### source

• `Optional` **source**: `string`

Menu source.

#### Defined in

[index.d.ts:17863](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17863)

___

### title

• **title**: `string` \| [`CommandActionTitle`](codearts_plugin_.CommandActionTitle.md)

Title show on menu.

#### Defined in

[index.d.ts:17838](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17838)

___

### toggled

• `Optional` **toggled**: `string` \| { `condition`: `string` ; `icon?`: [`MenuThemeIcon`](codearts_plugin_.MenuThemeIcon.md) ; `title?`: `string` ; `tooltip?`: `string`  }

ContextKey Expression.

#### Defined in

[index.d.ts:17873](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17873)

___

### tooltip

• `Optional` **tooltip**: `string`

Tooltip title.

#### Defined in

[index.d.ts:17853](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17853)
