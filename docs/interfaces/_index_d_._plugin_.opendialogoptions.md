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

*Defined in [index.d.ts:1855](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1855)*

Allow to select files, defaults to `true`.

___

### canSelectFolders

• `Optional` **canSelectFolders**: boolean

*Defined in [index.d.ts:1860](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1860)*

Allow to select folders, defaults to `false`.

___

### canSelectMany

• `Optional` **canSelectMany**: boolean

*Defined in [index.d.ts:1865](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1865)*

Allow to select many files or folders.

___

### defaultUri

• `Optional` **defaultUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:1845](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1845)*

The resource the dialog shows when opened.

___

### filters

• `Optional` **filters**: { [name:string]: string[];  }

*Defined in [index.d.ts:1877](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1877)*

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

*Defined in [index.d.ts:1850](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1850)*

A human-readable string for the open button.

___

### title

• `Optional` **title**: string

*Defined in [index.d.ts:1885](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1885)*

Dialog title.

This parameter might be ignored, as not all operating systems display a title on open dialogs
(for example, macOS).
