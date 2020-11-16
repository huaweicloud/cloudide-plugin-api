**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ThemeIcon

# Class: ThemeIcon

A reference to a named icon. Currently, [File](#ThemeIcon.File), [Folder](#ThemeIcon.Folder),
and [codicons](https://microsoft.github.io/vscode-codicons/dist/codicon.html) are supported.
Using a theme icon is preferred over a custom icon as it gives theme authors the possibility to change the icons.

*Note* that theme icons can also be rendered inside labels and descriptions. Places that support theme icons spell this out
and they use the `$(<name>)`-syntax, for instance `quickPick.label = "Hello World $(globe)"`.

## Hierarchy

* **ThemeIcon**

## Index

### Constructors

* [constructor](_index_d_._plugin_.themeicon.md#constructor)

### Properties

* [File](_index_d_._plugin_.themeicon.md#file)
* [Folder](_index_d_._plugin_.themeicon.md#folder)

## Constructors

### constructor

\+ **new ThemeIcon**(`id`: string): [ThemeIcon](_index_d_._plugin_.themeicon.md)

*Defined in [index.d.ts:817](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L817)*

Creates a reference to a theme icon.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | id of the icon. The available icons are listed in https://microsoft.github.io/vscode-codicons/dist/codicon.html.  |

**Returns:** [ThemeIcon](_index_d_._plugin_.themeicon.md)

## Properties

### File

▪ `Static` `Readonly` **File**: [ThemeIcon](_index_d_._plugin_.themeicon.md)

*Defined in [index.d.ts:812](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L812)*

Reference to an icon representing a file. The icon is taken from the current file icon theme or a placeholder icon is used.

___

### Folder

▪ `Static` `Readonly` **Folder**: [ThemeIcon](_index_d_._plugin_.themeicon.md)

*Defined in [index.d.ts:817](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L817)*

Reference to an icon representing a folder. The icon is taken from the current file icon theme or a placeholder icon is used.
