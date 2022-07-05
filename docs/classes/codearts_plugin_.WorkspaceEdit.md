[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WorkspaceEdit

# Class: WorkspaceEdit

["@codearts/plugin"](../modules/_codearts_plugin_.md).WorkspaceEdit

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

#### Defined in

[index.d.ts:3477](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L3477)

## Methods

### createFile

▸ **createFile**(`uri`, `options?`, `metadata?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) |  |
| `options?` | `Object` |  |
| `options.ignoreIfExists?` | `boolean` | - |
| `options.overwrite?` | `boolean` | - |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/codearts_plugin_.WorkspaceEditEntryMetadata.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:3542](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L3542)

___

### delete

▸ **delete**(`uri`, `range`, `metadata?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) |  |
| `range` | [`Range`](codearts_plugin_.Range.md) |  |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/codearts_plugin_.WorkspaceEditEntryMetadata.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:3506](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L3506)

___

### deleteFile

▸ **deleteFile**(`uri`, `options?`, `metadata?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) |  |
| `options?` | `Object` | - |
| `options.ignoreIfNotExists?` | `boolean` | - |
| `options.recursive?` | `boolean` | - |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/codearts_plugin_.WorkspaceEditEntryMetadata.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:3550](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L3550)

___

### entries

▸ **entries**(): [[`Uri`](codearts_plugin_.Uri.md), [`TextEdit`](codearts_plugin_.TextEdit.md)[]][]

#### Returns

[[`Uri`](codearts_plugin_.Uri.md), [`TextEdit`](codearts_plugin_.TextEdit.md)[]][]

#### Defined in

[index.d.ts:3568](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L3568)

___

### get

▸ **get**(`uri`): [`TextEdit`](codearts_plugin_.TextEdit.md)[]

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) |  |

#### Returns

[`TextEdit`](codearts_plugin_.TextEdit.md)[]

#### Defined in

[index.d.ts:3530](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L3530)

___

### has

▸ **has**(`uri`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) |  |

#### Returns

`boolean`

#### Defined in

[index.d.ts:3514](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L3514)

___

### insert

▸ **insert**(`uri`, `position`, `newText`, `metadata?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) |  |
| `position` | [`Position`](codearts_plugin_.Position.md) |  |
| `newText` | `string` |  |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/codearts_plugin_.WorkspaceEditEntryMetadata.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:3497](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L3497)

___

### renameFile

▸ **renameFile**(`oldUri`, `newUri`, `options?`, `metadata?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldUri` | [`Uri`](codearts_plugin_.Uri.md) |  |
| `newUri` | [`Uri`](codearts_plugin_.Uri.md) |  |
| `options?` | `Object` |  |
| `options.ignoreIfExists?` | `boolean` | - |
| `options.overwrite?` | `boolean` | - |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/codearts_plugin_.WorkspaceEditEntryMetadata.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:3561](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L3561)

___

### replace

▸ **replace**(`uri`, `range`, `newText`, `metadata?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) |  |
| `range` | [`Range`](codearts_plugin_.Range.md) |  |
| `newText` | `string` |  |
| `metadata?` | [`WorkspaceEditEntryMetadata`](../interfaces/codearts_plugin_.WorkspaceEditEntryMetadata.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:3487](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L3487)

___

### set

▸ **set**(`uri`, `edits`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) |  |
| `edits` | [`TextEdit`](codearts_plugin_.TextEdit.md)[] |  |

#### Returns

`void`

#### Defined in

[index.d.ts:3522](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L3522)
