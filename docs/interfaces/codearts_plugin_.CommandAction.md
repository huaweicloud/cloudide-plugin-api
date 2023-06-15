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

[index.d.ts:17739](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17739)

___

### icon

• `Optional` **icon**: [`MenuThemeIcon`](codearts_plugin_.MenuThemeIcon.md)

Menu icon.

#### Defined in

[index.d.ts:17749](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17749)

___

### id

• **id**: `string`

Command id.

#### Defined in

[index.d.ts:17724](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17724)

___

### precondition

• `Optional` **precondition**: `string`

ContextKey Expression.

#### Defined in

[index.d.ts:17759](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17759)

___

### shortTitle

• `Optional` **shortTitle**: `string`

Short title show on menu.

#### Defined in

[index.d.ts:17734](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17734)

___

### source

• `Optional` **source**: `string`

Menu source.

#### Defined in

[index.d.ts:17754](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17754)

___

### title

• **title**: `string` \| [`CommandActionTitle`](codearts_plugin_.CommandActionTitle.md)

Title show on menu.

#### Defined in

[index.d.ts:17729](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17729)

___

### toggled

• `Optional` **toggled**: `string` \| { `condition`: `string` ; `icon?`: [`MenuThemeIcon`](codearts_plugin_.MenuThemeIcon.md) ; `title?`: `string` ; `tooltip?`: `string`  }

ContextKey Expression.

#### Defined in

[index.d.ts:17764](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17764)

___

### tooltip

• `Optional` **tooltip**: `string`

Tooltip title.

#### Defined in

[index.d.ts:17744](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L17744)
