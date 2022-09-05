[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SaveDialogOptions

# Interface: SaveDialogOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).SaveDialogOptions

Options to configure the behaviour of a file save dialog.

## Table of contents

### Properties

- [defaultUri](codearts_plugin_.SaveDialogOptions.md#defaulturi)
- [filters](codearts_plugin_.SaveDialogOptions.md#filters)
- [saveLabel](codearts_plugin_.SaveDialogOptions.md#savelabel)
- [title](codearts_plugin_.SaveDialogOptions.md#title)

## Properties

### defaultUri

• `Optional` **defaultUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The resource the dialog shows when opened.

#### Defined in

[index.d.ts:1912](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1912)

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

[index.d.ts:1929](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1929)

___

### saveLabel

• `Optional` **saveLabel**: `string`

A human-readable string for the save button.

#### Defined in

[index.d.ts:1917](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1917)

___

### title

• `Optional` **title**: `string`

Dialog title.

This parameter might be ignored, as not all operating systems display a title on save dialogs
(for example, macOS).

#### Defined in

[index.d.ts:1937](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1937)
