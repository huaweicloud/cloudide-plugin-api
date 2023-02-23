[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / OpenDialogOptions

# Interface: OpenDialogOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).OpenDialogOptions

Options to configure the behaviour of a file open dialog.

* Note 1: A dialog can select files, folders, or both. This is not true for Windows
which enforces to open either files or folder, but *not both*.
* Note 2: Explicitly setting `canSelectFiles` and `canSelectFolders` to `false` is futile
and the editor then silently adjusts the options to select files.

## Table of contents

### Properties

- [canSelectFiles](cloudide_plugin_.OpenDialogOptions.md#canselectfiles)
- [canSelectFolders](cloudide_plugin_.OpenDialogOptions.md#canselectfolders)
- [canSelectMany](cloudide_plugin_.OpenDialogOptions.md#canselectmany)
- [defaultUri](cloudide_plugin_.OpenDialogOptions.md#defaulturi)
- [filters](cloudide_plugin_.OpenDialogOptions.md#filters)
- [openLabel](cloudide_plugin_.OpenDialogOptions.md#openlabel)
- [title](cloudide_plugin_.OpenDialogOptions.md#title)

## Properties

### canSelectFiles

• `Optional` **canSelectFiles**: `boolean`

Allow to select files, defaults to `true`.

#### Defined in

[index.d.ts:2669](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2669)

___

### canSelectFolders

• `Optional` **canSelectFolders**: `boolean`

Allow to select folders, defaults to `false`.

#### Defined in

[index.d.ts:2674](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2674)

___

### canSelectMany

• `Optional` **canSelectMany**: `boolean`

Allow to select many files or folders.

#### Defined in

[index.d.ts:2679](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2679)

___

### defaultUri

• `Optional` **defaultUri**: [`Uri`](../classes/cloudide_plugin_.Uri.md)

The resource the dialog shows when opened.

#### Defined in

[index.d.ts:2659](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2659)

___

### filters

• `Optional` **filters**: `Object`

A set of file filters that are used by the dialog. Each entry is a human readable label,
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

[index.d.ts:2691](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2691)

___

### openLabel

• `Optional` **openLabel**: `string`

A human-readable string for the open button.

#### Defined in

[index.d.ts:2664](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2664)

___

### title

• `Optional` **title**: `string`

Dialog title.
This parameter might be ignored, as not all operating systems display a title on open dialogs.

#### Defined in

[index.d.ts:2654](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2654)
