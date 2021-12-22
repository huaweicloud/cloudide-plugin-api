**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / OpenDialogOptions

# Interface: OpenDialogOptions

Options to configure the behaviour of a file open dialog.

* Note 1: On Windows and Linux, a file dialog cannot be both a file selector and a folder selector, so if you
set both `canSelectFiles` and `canSelectFolders` to `true` on these platforms, a folder selector will be shown.
* Note 2: Explicitly setting `canSelectFiles` and `canSelectFolders` to `false` is futile
and the editor then silently adjusts the options to select files.

## Hierarchy

* **OpenDialogOptions**

## Index

### Properties

* [canSelectFiles](_index_d_._plugin_.opendialogoptions.md#canselectfiles)
* [canSelectFolders](_index_d_._plugin_.opendialogoptions.md#canselectfolders)
* [canSelectMany](_index_d_._plugin_.opendialogoptions.md#canselectmany)
* [defaultUri](_index_d_._plugin_.opendialogoptions.md#defaulturi)
* [filters](_index_d_._plugin_.opendialogoptions.md#filters)
* [openLabel](_index_d_._plugin_.opendialogoptions.md#openlabel)
* [title](_index_d_._plugin_.opendialogoptions.md#title)

## Properties

### canSelectFiles

• `Optional` **canSelectFiles**: boolean

*Defined in [index.d.ts:1858](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1858)*

Allow to select files, defaults to `true`.

___

### canSelectFolders

• `Optional` **canSelectFolders**: boolean

*Defined in [index.d.ts:1863](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1863)*

Allow to select folders, defaults to `false`.

___

### canSelectMany

• `Optional` **canSelectMany**: boolean

*Defined in [index.d.ts:1868](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1868)*

Allow to select many files or folders.

___

### defaultUri

• `Optional` **defaultUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:1848](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1848)*

The resource the dialog shows when opened.

___

### filters

• `Optional` **filters**: { [name:string]: string[];  }

*Defined in [index.d.ts:1880](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1880)*

A set of file filters that are used by the dialog. Each entry is a human-readable label,
like "TypeScript", and an array of extensions, e.g.
```ts
{
	'Images': ['png', 'jpg']
	'TypeScript': ['ts', 'tsx']
}
```

___

### openLabel

• `Optional` **openLabel**: string

*Defined in [index.d.ts:1853](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1853)*

A human-readable string for the open button.

___

### title

• `Optional` **title**: string

*Defined in [index.d.ts:1888](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1888)*

Dialog title.

This parameter might be ignored, as not all operating systems display a title on open dialogs
(for example, macOS).
