[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ThemeIcon

# Class: ThemeIcon

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ThemeIcon

A reference to a named icon. Currently only [File](#ThemeIcon.File) and [Folder](#ThemeIcon.Folder) are supported.
Using a theme icon is preferred over a custom icon as it gives theme authors the possibility to change the icons.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.ThemeIcon.md#constructor)

### Properties

- [id](cloudide_plugin_.ThemeIcon.md#id)
- [File](cloudide_plugin_.ThemeIcon.md#file)
- [Folder](cloudide_plugin_.ThemeIcon.md#folder)

## Constructors

### constructor

• `Private` **new ThemeIcon**(`id`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |

#### Defined in

[index.d.ts:2579](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2579)

## Properties

### id

• **id**: `string`

#### Defined in

[index.d.ts:2579](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2579)

___

### File

▪ `Static` `Readonly` **File**: [`ThemeIcon`](cloudide_plugin_.ThemeIcon.md)

Reference to a icon representing a file. The icon is taken from the current file icon theme or a placeholder icon.

#### Defined in

[index.d.ts:2572](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2572)

___

### Folder

▪ `Static` `Readonly` **Folder**: [`ThemeIcon`](cloudide_plugin_.ThemeIcon.md)

Reference to a icon representing a folder. The icon is taken from the current file icon theme or a placeholder icon.

#### Defined in

[index.d.ts:2577](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2577)
