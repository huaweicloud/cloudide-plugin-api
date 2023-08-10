[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WorkspaceEdit

# Class: WorkspaceEdit

["@codearts/plugin"](../modules/_codearts_plugin_.md).WorkspaceEdit

A workspace edit is a collection of textual and files changes for
multiple resources and documents.

Use the [applyEdit](../modules/codearts_plugin_.workspace.md#applyedit)-function to apply a workspace edit.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.WorkspaceEdit.md#constructor)

### Properties

- [size](codearts_plugin_.WorkspaceEdit.md#size)

### Methods

- [createFile](codearts_plugin_.WorkspaceEdit.md#createfile)
- [delete](codearts_plugin_.WorkspaceEdit.md#delete)
- [deleteFile](codearts_plugin_.WorkspaceEdit.md#deletefile)
- [entries](codearts_plugin_.WorkspaceEdit.md#entries)
- [get](codearts_plugin_.WorkspaceEdit.md#get)
- [has](codearts_plugin_.WorkspaceEdit.md#has)
- [insert](codearts_plugin_.WorkspaceEdit.md#insert)
- [renameFile](codearts_plugin_.WorkspaceEdit.md#renamefile)
- [replace](codearts_plugin_.WorkspaceEdit.md#replace)
- [set](codearts_plugin_.WorkspaceEdit.md#set)

## Constructors

### constructor

• **new WorkspaceEdit**()

## Properties

### size

• `Readonly` **size**: `number`

The number of affected resources of textual or resource changes.

#### Defined in

[index.d.ts:3515](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3515)

## Methods

### createFile

▸ **createFile**(`uri`, `options?`, `metadata?`): `void`

Create a regular file.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) | Uri of the new file.. |
| `options?` | `Object` | Defines if an existing file should be overwritten or be ignored. When overwrite and ignoreIfExists are both set overwrite wins. When both are unset and when the file already exists then the edit cannot be applied successfully. |
| `options.ignoreIfExists?` | `boolean` | - |
| `options.overwrite?` | `boolean` | - |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/codearts_plugin_.WorkspaceEditEntryMetadata.md) | Optional metadata for the entry. |

#### Returns

`void`

#### Defined in

[index.d.ts:3580](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3580)

___

### delete

▸ **delete**(`uri`, `range`, `metadata?`): `void`

Delete the text at the given range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) | A resource identifier. |
| `range` | [`Range`](codearts_plugin_.Range.md) | A range. |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/codearts_plugin_.WorkspaceEditEntryMetadata.md) | Optional metadata for the entry. |

#### Returns

`void`

#### Defined in

[index.d.ts:3544](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3544)

___

### deleteFile

▸ **deleteFile**(`uri`, `options?`, `metadata?`): `void`

Delete a file or folder.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) | The uri of the file that is to be deleted. |
| `options?` | `Object` | - |
| `options.ignoreIfNotExists?` | `boolean` | - |
| `options.recursive?` | `boolean` | - |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/codearts_plugin_.WorkspaceEditEntryMetadata.md) | Optional metadata for the entry. |

#### Returns

`void`

#### Defined in

[index.d.ts:3588](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3588)

___

### entries

▸ **entries**(): [[`Uri`](codearts_plugin_.Uri.md), [`TextEdit`](codearts_plugin_.TextEdit.md)[]][]

Get all text edits grouped by resource.

#### Returns

[[`Uri`](codearts_plugin_.Uri.md), [`TextEdit`](codearts_plugin_.TextEdit.md)[]][]

A shallow copy of `[Uri, TextEdit[]]`-tuples.

#### Defined in

[index.d.ts:3606](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3606)

___

### get

▸ **get**(`uri`): [`TextEdit`](codearts_plugin_.TextEdit.md)[]

Get the text edits for a resource.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) | A resource identifier. |

#### Returns

[`TextEdit`](codearts_plugin_.TextEdit.md)[]

An array of text edits.

#### Defined in

[index.d.ts:3568](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3568)

___

### has

▸ **has**(`uri`): `boolean`

Check if a text edit for a resource exists.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) | A resource identifier. |

#### Returns

`boolean`

`true` if the given resource will be touched by this edit.

#### Defined in

[index.d.ts:3552](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3552)

___

### insert

▸ **insert**(`uri`, `position`, `newText`, `metadata?`): `void`

Insert the given text at the given position.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) | A resource identifier. |
| `position` | [`Position`](codearts_plugin_.Position.md) | A position. |
| `newText` | `string` | A string. |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/codearts_plugin_.WorkspaceEditEntryMetadata.md) | Optional metadata for the entry. |

#### Returns

`void`

#### Defined in

[index.d.ts:3535](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3535)

___

### renameFile

▸ **renameFile**(`oldUri`, `newUri`, `options?`, `metadata?`): `void`

Rename a file or folder.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldUri` | [`Uri`](codearts_plugin_.Uri.md) | The existing file. |
| `newUri` | [`Uri`](codearts_plugin_.Uri.md) | The new location. |
| `options?` | `Object` | Defines if existing files should be overwritten or be ignored. When overwrite and ignoreIfExists are both set overwrite wins. |
| `options.ignoreIfExists?` | `boolean` | - |
| `options.overwrite?` | `boolean` | - |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/codearts_plugin_.WorkspaceEditEntryMetadata.md) | Optional metadata for the entry. |

#### Returns

`void`

#### Defined in

[index.d.ts:3599](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3599)

___

### replace

▸ **replace**(`uri`, `range`, `newText`, `metadata?`): `void`

Replace the given range with given text for the given resource.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) | A resource identifier. |
| `range` | [`Range`](codearts_plugin_.Range.md) | A range. |
| `newText` | `string` | A string. |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/codearts_plugin_.WorkspaceEditEntryMetadata.md) | Optional metadata for the entry. |

#### Returns

`void`

#### Defined in

[index.d.ts:3525](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3525)

___

### set

▸ **set**(`uri`, `edits`): `void`

Set (and replace) text edits for a resource.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) | A resource identifier. |
| `edits` | [`TextEdit`](codearts_plugin_.TextEdit.md)[] | An array of text edits. |

#### Returns

`void`

#### Defined in

[index.d.ts:3560](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L3560)
