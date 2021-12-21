**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ThemeIcon

# Class: ThemeIcon

A reference to a named icon. Currently, [File](#ThemeIcon.File), [Folder](#ThemeIcon.Folder),
and [ThemeIcon ids](https://code.visualstudio.com/api/references/icons-in-labels#icon-listing) are supported.
Using a theme icon is preferred over a custom icon as it gives product theme authors the possibility to change the icons.

*Note* that theme icons can also be rendered inside labels and descriptions. Places that support theme icons spell this out
and they use the `$(<name>)`-syntax, for instance `quickPick.label = "Hello World $(globe)"`.

## Hierarchy

* **ThemeIcon**

## Index

### Constructors

* [constructor](_index_d_._plugin_.themeicon.md#constructor)

### Properties

* [color](_index_d_._plugin_.themeicon.md#color)
* [id](_index_d_._plugin_.themeicon.md#id)
* [File](_index_d_._plugin_.themeicon.md#file)
* [Folder](_index_d_._plugin_.themeicon.md#folder)

## Constructors

### constructor

\+ **new ThemeIcon**(`id`: string, `color?`: [ThemeColor](_index_d_._plugin_.themecolor.md)): [ThemeIcon](_index_d_._plugin_.themeicon.md)

*Defined in [index.d.ts:937](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L937)*

Creates a reference to a theme icon.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | id of the icon. The available icons are listed in https://code.visualstudio.com/api/references/icons-in-labels#icon-listing. |
`color?` | [ThemeColor](_index_d_._plugin_.themecolor.md) | optional `ThemeColor` for the icon. The color is currently only used in [TreeItem](#TreeItem).  |

**Returns:** [ThemeIcon](_index_d_._plugin_.themeicon.md)

## Properties

### color

• `Optional` `Readonly` **color**: [ThemeColor](_index_d_._plugin_.themecolor.md)

*Defined in [index.d.ts:937](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L937)*

The optional ThemeColor of the icon. The color is currently only used in [TreeItem](#TreeItem).

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:932](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L932)*

The id of the icon. The available icons are listed in https://code.visualstudio.com/api/references/icons-in-labels#icon-listing.

___

### File

▪ `Static` `Readonly` **File**: [ThemeIcon](_index_d_._plugin_.themeicon.md)

*Defined in [index.d.ts:922](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L922)*

Reference to an icon representing a file. The icon is taken from the current file icon theme or a placeholder icon is used.

___

### Folder

▪ `Static` `Readonly` **Folder**: [ThemeIcon](_index_d_._plugin_.themeicon.md)

*Defined in [index.d.ts:927](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L927)*

Reference to an icon representing a folder. The icon is taken from the current file icon theme or a placeholder icon is used.
