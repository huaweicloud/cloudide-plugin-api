[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / WorkspaceEdit

# Class: WorkspaceEdit

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).WorkspaceEdit

A workspace edit is a collection of textual and files changes for
multiple resources and documents.

Use the [applyEdit](#workspace.applyEdit)-function to apply a workspace edit.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.WorkspaceEdit.md#constructor)

### Properties

- [size](cloudide_plugin_.WorkspaceEdit.md#size)

### Methods

- [createFile](cloudide_plugin_.WorkspaceEdit.md#createfile)
- [delete](cloudide_plugin_.WorkspaceEdit.md#delete)
- [deleteFile](cloudide_plugin_.WorkspaceEdit.md#deletefile)
- [entries](cloudide_plugin_.WorkspaceEdit.md#entries)
- [get](cloudide_plugin_.WorkspaceEdit.md#get)
- [has](cloudide_plugin_.WorkspaceEdit.md#has)
- [insert](cloudide_plugin_.WorkspaceEdit.md#insert)
- [renameFile](cloudide_plugin_.WorkspaceEdit.md#renamefile)
- [replace](cloudide_plugin_.WorkspaceEdit.md#replace)
- [set](cloudide_plugin_.WorkspaceEdit.md#set)

## Constructors

### constructor

• **new WorkspaceEdit**()

## Properties

### size

• `Readonly` **size**: `number`

The number of affected resources of textual or resource changes.

#### Defined in

[index.d.ts:8247](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8247)

## Methods

### createFile

▸ **createFile**(`uri`, `options?`, `metadata?`): `void`

Create a regular file.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](cloudide_plugin_.Uri.md) | Uri of the new file.. |
| `options?` | `Object` | Defines if an existing file should be overwritten or be ignored. When overwrite and ignoreIfExists are both set overwrite wins. |
| `options.ignoreIfExists?` | `boolean` | - |
| `options.overwrite?` | `boolean` | - |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/cloudide_plugin_.WorkspaceEditEntryMetadata.md) | Optional metadata for the entry. |

#### Returns

`void`

#### Defined in

[index.d.ts:8310](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8310)

___

### delete

▸ **delete**(`uri`, `range`, `metadata?`): `void`

Delete the text at the given range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](cloudide_plugin_.Uri.md) | A resource identifier. |
| `range` | [`Range`](cloudide_plugin_.Range.md) | A range. |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/cloudide_plugin_.WorkspaceEditEntryMetadata.md) | Optional metadata for the entry. |

#### Returns

`void`

#### Defined in

[index.d.ts:8276](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8276)

___

### deleteFile

▸ **deleteFile**(`uri`, `options?`, `metadata?`): `void`

Delete a file or folder.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](cloudide_plugin_.Uri.md) | The uri of the file that is to be deleted. |
| `options?` | `Object` | - |
| `options.ignoreIfNotExists?` | `boolean` | - |
| `options.recursive?` | `boolean` | - |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/cloudide_plugin_.WorkspaceEditEntryMetadata.md) | Optional metadata for the entry. |

#### Returns

`void`

#### Defined in

[index.d.ts:8318](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8318)

___

### entries

▸ **entries**(): [[`Uri`](cloudide_plugin_.Uri.md), [`TextEdit`](cloudide_plugin_.TextEdit.md)[]][]

Get all text edits grouped by resource.

#### Returns

[[`Uri`](cloudide_plugin_.Uri.md), [`TextEdit`](cloudide_plugin_.TextEdit.md)[]][]

A shallow copy of `[Uri, TextEdit[]]`-tuples.

#### Defined in

[index.d.ts:8336](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8336)

___

### get

▸ **get**(`uri`): [`TextEdit`](cloudide_plugin_.TextEdit.md)[]

Get the text edits for a resource.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](cloudide_plugin_.Uri.md) | A resource identifier. |

#### Returns

[`TextEdit`](cloudide_plugin_.TextEdit.md)[]

An array of text edits.

#### Defined in

[index.d.ts:8300](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8300)

___

### has

▸ **has**(`uri`): `boolean`

Check if a text edit for a resource exists.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](cloudide_plugin_.Uri.md) | A resource identifier. |

#### Returns

`boolean`

`true` if the given resource will be touched by this edit.

#### Defined in

[index.d.ts:8284](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8284)

___

### insert

▸ **insert**(`uri`, `position`, `newText`, `metadata?`): `void`

Insert the given text at the given position.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](cloudide_plugin_.Uri.md) | A resource identifier. |
| `position` | [`Position`](cloudide_plugin_.Position.md) | A position. |
| `newText` | `string` | A string. |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/cloudide_plugin_.WorkspaceEditEntryMetadata.md) | Optional metadata for the entry. |

#### Returns

`void`

#### Defined in

[index.d.ts:8267](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8267)

___

### renameFile

▸ **renameFile**(`oldUri`, `newUri`, `options?`, `metadata?`): `void`

Rename a file or folder.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldUri` | [`Uri`](cloudide_plugin_.Uri.md) | The existing file. |
| `newUri` | [`Uri`](cloudide_plugin_.Uri.md) | The new location. |
| `options?` | `Object` | Defines if existing files should be overwritten or be ignored. When overwrite and ignoreIfExists are both set overwrite wins. |
| `options.ignoreIfExists?` | `boolean` | - |
| `options.overwrite?` | `boolean` | - |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/cloudide_plugin_.WorkspaceEditEntryMetadata.md) | Optional metadata for the entry. |

#### Returns

`void`

#### Defined in

[index.d.ts:8329](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8329)

___

### replace

▸ **replace**(`uri`, `range`, `newText`, `metadata?`): `void`

Replace the given range with given text for the given resource.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](cloudide_plugin_.Uri.md) | A resource identifier. |
| `range` | [`Range`](cloudide_plugin_.Range.md) | A range. |
| `newText` | `string` | A string. |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/cloudide_plugin_.WorkspaceEditEntryMetadata.md) | Optional metadata for the entry. |

#### Returns

`void`

#### Defined in

[index.d.ts:8257](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8257)

___

### set

▸ **set**(`uri`, `edits`): `void`

Set (and replace) text edits for a resource.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](cloudide_plugin_.Uri.md) | A resource identifier. |
| `edits` | [`TextEdit`](cloudide_plugin_.TextEdit.md)[] | An array of text edits. |

#### Returns

`void`

#### Defined in

[index.d.ts:8292](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8292)
