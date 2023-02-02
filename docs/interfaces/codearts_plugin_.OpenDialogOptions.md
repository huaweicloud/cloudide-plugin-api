[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / OpenDialogOptions

# Interface: OpenDialogOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).OpenDialogOptions

Options to configure the behaviour of a file open dialog.

* Note 1: On Windows and Linux, a file dialog cannot be both a file selector and a folder selector, so if you
set both `canSelectFiles` and `canSelectFolders` to `true` on these platforms, a folder selector will be shown.
* Note 2: Explicitly setting `canSelectFiles` and `canSelectFolders` to `false` is futile
and the editor then silently adjusts the options to select files.

## Table of contents

### Properties

- [canSelectFiles](codearts_plugin_.OpenDialogOptions.md#canselectfiles)
- [canSelectFolders](codearts_plugin_.OpenDialogOptions.md#canselectfolders)
- [canSelectMany](codearts_plugin_.OpenDialogOptions.md#canselectmany)
- [defaultUri](codearts_plugin_.OpenDialogOptions.md#defaulturi)
- [filters](codearts_plugin_.OpenDialogOptions.md#filters)
- [openLabel](codearts_plugin_.OpenDialogOptions.md#openlabel)
- [title](codearts_plugin_.OpenDialogOptions.md#title)

## Properties

### canSelectFiles

• `Optional` **canSelectFiles**: `boolean`

Allow to select files, defaults to `true`.

#### Defined in

[index.d.ts:1872](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1872)

___

### canSelectFolders

• `Optional` **canSelectFolders**: `boolean`

Allow to select folders, defaults to `false`.

#### Defined in

[index.d.ts:1877](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1877)

___

### canSelectMany

• `Optional` **canSelectMany**: `boolean`

Allow to select many files or folders.

#### Defined in

[index.d.ts:1882](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1882)

___

### defaultUri

• `Optional` **defaultUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The resource the dialog shows when opened.

#### Defined in

[index.d.ts:1862](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1862)

___

### filters

• `Optional` **filters**: `Object`

A set of file filters that are used by the dialog. Each entry is a human-readable label,
like "TypeScript", and an array of extensions, e.g.
```ts
{
	'Images': ['png', 'jpg']
	'TypeScript': ['ts', 'tsx']
}
```

#### Index signature

▪ [name: `string`]: `string`[]

#### Defined in

[index.d.ts:1894](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1894)

___

### openLabel

• `Optional` **openLabel**: `string`

A human-readable string for the open button.

#### Defined in

[index.d.ts:1867](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1867)

___

### title

• `Optional` **title**: `string`

Dialog title.

This parameter might be ignored, as not all operating systems display a title on open dialogs
(for example, macOS).

#### Defined in

[index.d.ts:1902](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1902)
