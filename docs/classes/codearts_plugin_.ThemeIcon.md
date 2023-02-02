[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ThemeIcon

# Class: ThemeIcon

["@codearts/plugin"](../modules/_codearts_plugin_.md).ThemeIcon

A reference to a named icon. Currently, [File](codearts_plugin_.ThemeIcon.md#file), [Folder](codearts_plugin_.ThemeIcon.md#folder),
and [ThemeIcon ids](https://code.visualstudio.com/api/references/icons-in-labels#icon-listing) are supported.
Using a theme icon is preferred over a custom icon as it gives product theme authors the possibility to change the icons.

*Note* that theme icons can also be rendered inside labels and descriptions. Places that support theme icons spell this out
and they use the `$(<name>)`-syntax, for instance `quickPick.label = "Hello World $(globe)"`.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.ThemeIcon.md#constructor)

### Properties

- [color](codearts_plugin_.ThemeIcon.md#color)
- [id](codearts_plugin_.ThemeIcon.md#id)
- [File](codearts_plugin_.ThemeIcon.md#file)
- [Folder](codearts_plugin_.ThemeIcon.md#folder)

## Constructors

### constructor

• **new ThemeIcon**(`id`, `color?`)

Creates a reference to a theme icon.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | id of the icon. The available icons are listed in https://code.visualstudio.com/api/references/icons-in-labels#icon-listing. |
| `color?` | [`ThemeColor`](codearts_plugin_.ThemeColor.md) | optional `ThemeColor` for the icon. The color is currently only used in [TreeItem](codearts_plugin_.TreeItem.md). |

#### Defined in

[index.d.ts:897](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L897)

## Properties

### color

• `Optional` `Readonly` **color**: [`ThemeColor`](codearts_plugin_.ThemeColor.md)

The optional ThemeColor of the icon. The color is currently only used in [TreeItem](codearts_plugin_.TreeItem.md).

#### Defined in

[index.d.ts:890](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L890)

___

### id

• `Readonly` **id**: `string`

The id of the icon. The available icons are listed in https://code.visualstudio.com/api/references/icons-in-labels#icon-listing.

#### Defined in

[index.d.ts:885](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L885)

___

### File

▪ `Static` `Readonly` **File**: [`ThemeIcon`](codearts_plugin_.ThemeIcon.md)

Reference to an icon representing a file. The icon is taken from the current file icon theme or a placeholder icon is used.

#### Defined in

[index.d.ts:875](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L875)

___

### Folder

▪ `Static` `Readonly` **Folder**: [`ThemeIcon`](codearts_plugin_.ThemeIcon.md)

Reference to an icon representing a folder. The icon is taken from the current file icon theme or a placeholder icon is used.

#### Defined in

[index.d.ts:880](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L880)
