[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SaveDialogOptions

# Interface: SaveDialogOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SaveDialogOptions

Options to configure the behaviour of a file save dialog.

## Table of contents

### Properties

- [defaultUri](cloudide_plugin_.SaveDialogOptions.md#defaulturi)
- [filters](cloudide_plugin_.SaveDialogOptions.md#filters)
- [saveLabel](cloudide_plugin_.SaveDialogOptions.md#savelabel)
- [title](cloudide_plugin_.SaveDialogOptions.md#title)

## Properties

### defaultUri

• `Optional` **defaultUri**: [`Uri`](../classes/cloudide_plugin_.Uri.md)

The resource the dialog shows when opened.

#### Defined in

[index.d.ts:2708](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2708)

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

[index.d.ts:2725](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2725)

___

### saveLabel

• `Optional` **saveLabel**: `string`

A human-readable string for the save button.

#### Defined in

[index.d.ts:2713](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2713)

___

### title

• `Optional` **title**: `string`

Dialog title.
This parameter might be ignored, as not all operating systems display a title on save dialogs.

#### Defined in

[index.d.ts:2703](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2703)
