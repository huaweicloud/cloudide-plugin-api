[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / FileSystem

# Interface: FileSystem

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).FileSystem

The file system interface exposes the editor's built-in and contributed
[file system providers](#FileSystemProvider). It allows extensions to work
with files from the local disk as well as files from remote places, like the
remote extension host or ftp-servers.

*Note* that an instance of this interface is available as [`workspace.fs`](#workspace.fs).

## Table of contents

### Methods

- [copy](cloudide_plugin_.FileSystem.md#copy)
- [createDirectory](cloudide_plugin_.FileSystem.md#createdirectory)
- [delete](cloudide_plugin_.FileSystem.md#delete)
- [readDirectory](cloudide_plugin_.FileSystem.md#readdirectory)
- [readFile](cloudide_plugin_.FileSystem.md#readfile)
- [rename](cloudide_plugin_.FileSystem.md#rename)
- [stat](cloudide_plugin_.FileSystem.md#stat)
- [writeFile](cloudide_plugin_.FileSystem.md#writefile)

## Methods

### copy

▸ **copy**(`source`, `target`, `options?`): [`Thenable`](Thenable.md)<`void`\>

Copy files or folders.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The existing file. |
| `target` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | - |
| `options?` | `Object` | Defines if existing files should be overwritten. |
| `options.overwrite?` | `boolean` | - |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:5957](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5957)

___

### createDirectory

▸ **createDirectory**(`uri`): [`Thenable`](Thenable.md)<`void`\>

Create a new directory (Note, that new files are created via `write`-calls).

*Note* that missing directories are created automatically, e.g this call has
`mkdirp` semantics.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The uri of the new folder. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:5915](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5915)

___

### delete

▸ **delete**(`uri`, `options?`): [`Thenable`](Thenable.md)<`void`\>

Delete a file.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The resource that is to be deleted. |
| `options?` | `Object` | Defines if trash can should be used and if deletion of folders is recursive |
| `options.recursive?` | `boolean` | - |
| `options.useTrash?` | `boolean` | - |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:5939](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5939)

___

### readDirectory

▸ **readDirectory**(`uri`): [`Thenable`](Thenable.md)<[`string`, [`FileType`](../enums/cloudide_plugin_.FileType.md)][]\>

Retrieve all entries of a [directory](#FileType.Directory).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The uri of the folder. |

#### Returns

[`Thenable`](Thenable.md)<[`string`, [`FileType`](../enums/cloudide_plugin_.FileType.md)][]\>

An array of name/type-tuples or a thenable that resolves to such.

#### Defined in

[index.d.ts:5905](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5905)

___

### readFile

▸ **readFile**(`uri`): [`Thenable`](Thenable.md)<`Uint8Array`\>

Read the entire contents of a file.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The uri of the file. |

#### Returns

[`Thenable`](Thenable.md)<`Uint8Array`\>

An array of bytes or a thenable that resolves to such.

#### Defined in

[index.d.ts:5923](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5923)

___

### rename

▸ **rename**(`source`, `target`, `options?`): [`Thenable`](Thenable.md)<`void`\>

Rename a file or folder.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | - |
| `target` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | - |
| `options?` | `Object` | Defines if existing files should be overwritten. |
| `options.overwrite?` | `boolean` | - |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:5948](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5948)

___

### stat

▸ **stat**(`uri`): [`Thenable`](Thenable.md)<[`FileStat`](cloudide_plugin_.FileStat.md)\>

Retrieve metadata about a file.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The uri of the file to retrieve metadata about. |

#### Returns

[`Thenable`](Thenable.md)<[`FileStat`](cloudide_plugin_.FileStat.md)\>

The file metadata about the file.

#### Defined in

[index.d.ts:5897](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5897)

___

### writeFile

▸ **writeFile**(`uri`, `content`): [`Thenable`](Thenable.md)<`void`\>

Write data to a file, replacing its entire contents.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The uri of the file. |
| `content` | `Uint8Array` | The new content of the file. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:5931](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5931)
