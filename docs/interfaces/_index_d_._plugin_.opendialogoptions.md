**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / OpenDialogOptions

# Interface: OpenDialogOptions

Options to configure the behaviour of a file open dialog.

* Note 1: A dialog can select files, folders, or both. This is not true for Windows
which enforces to open either files or folder, but *not both*.
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

## Properties

### canSelectFiles

• `Optional` **canSelectFiles**: boolean

*Defined in [index.d.ts:1718](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1718)*

Allow to select files, defaults to `true`.

___

### canSelectFolders

• `Optional` **canSelectFolders**: boolean

*Defined in [index.d.ts:1723](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1723)*

Allow to select folders, defaults to `false`.

___

### canSelectMany

• `Optional` **canSelectMany**: boolean

*Defined in [index.d.ts:1728](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1728)*

Allow to select many files or folders.

___

### defaultUri

• `Optional` **defaultUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:1708](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1708)*

The resource the dialog shows when opened.

___

### filters

• `Optional` **filters**: { [name:string]: string[];  }

*Defined in [index.d.ts:1740](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1740)*

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

*Defined in [index.d.ts:1713](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1713)*

A human-readable string for the open button.
