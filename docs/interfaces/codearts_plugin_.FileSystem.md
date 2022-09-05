[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileSystem

# Interface: FileSystem

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileSystem

The file system interface exposes the editor's built-in and contributed
[file system providers](codearts_plugin_.FileSystemProvider.md). It allows extensions to work
with files from the local disk as well as files from remote places, like the
remote extension host or ftp-servers.

*Note* that an instance of this interface is available as [`fs`](../modules/codearts_plugin_.workspace.md#fs).

## Table of contents

### Methods

- [copy](codearts_plugin_.FileSystem.md#copy)
- [createDirectory](codearts_plugin_.FileSystem.md#createdirectory)
- [delete](codearts_plugin_.FileSystem.md#delete)
- [isWritableFileSystem](codearts_plugin_.FileSystem.md#iswritablefilesystem)
- [readDirectory](codearts_plugin_.FileSystem.md#readdirectory)
- [readFile](codearts_plugin_.FileSystem.md#readfile)
- [rename](codearts_plugin_.FileSystem.md#rename)
- [stat](codearts_plugin_.FileSystem.md#stat)
- [writeFile](codearts_plugin_.FileSystem.md#writefile)

## Methods

### copy

▸ **copy**(`source`, `target`, `options?`): [`Thenable`](Thenable.md)<`void`\>

Copy files or folders.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The existing file. |
| `target` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The destination location. |
| `options?` | `Object` | Defines if existing files should be overwritten. |
| `options.overwrite?` | `boolean` | - |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8158](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8158)

___

### createDirectory

▸ **createDirectory**(`uri`): [`Thenable`](Thenable.md)<`void`\>

Create a new directory (Note, that new files are created via `write`-calls).

*Note* that missing directories are created automatically, e.g this call has
`mkdirp` semantics.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The uri of the new folder. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8116](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8116)

___

### delete

▸ **delete**(`uri`, `options?`): [`Thenable`](Thenable.md)<`void`\>

Delete a file.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The resource that is to be deleted. |
| `options?` | `Object` | Defines if trash can should be used and if deletion of folders is recursive |
| `options.recursive?` | `boolean` | - |
| `options.useTrash?` | `boolean` | - |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8140](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8140)

___

### isWritableFileSystem

▸ **isWritableFileSystem**(`scheme`): `undefined` \| `boolean`

Check if a given file system supports writing files.

Keep in mind that just because a file system supports writing, that does
not mean that writes will always succeed. There may be permissions issues
or other errors that prevent writing a file.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scheme` | `string` | The scheme of the filesystem, for example `file` or `git`. |

#### Returns

`undefined` \| `boolean`

`true` if the file system supports writing, `false` if it does not
support writing (i.e. it is readonly), and `undefined` if the editor does not
know about the filesystem.

#### Defined in

[index.d.ts:8173](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8173)

___

### readDirectory

▸ **readDirectory**(`uri`): [`Thenable`](Thenable.md)<[`string`, [`FileType`](../enums/codearts_plugin_.FileType.md)][]\>

Retrieve all entries of a [directory](../enums/codearts_plugin_.FileType.md#directory).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The uri of the folder. |

#### Returns

[`Thenable`](Thenable.md)<[`string`, [`FileType`](../enums/codearts_plugin_.FileType.md)][]\>

An array of name/type-tuples or a thenable that resolves to such.

#### Defined in

[index.d.ts:8106](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8106)

___

### readFile

▸ **readFile**(`uri`): [`Thenable`](Thenable.md)<`Uint8Array`\>

Read the entire contents of a file.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The uri of the file. |

#### Returns

[`Thenable`](Thenable.md)<`Uint8Array`\>

An array of bytes or a thenable that resolves to such.

#### Defined in

[index.d.ts:8124](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8124)

___

### rename

▸ **rename**(`source`, `target`, `options?`): [`Thenable`](Thenable.md)<`void`\>

Rename a file or folder.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The existing file. |
| `target` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The new location. |
| `options?` | `Object` | Defines if existing files should be overwritten. |
| `options.overwrite?` | `boolean` | - |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8149](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8149)

___

### stat

▸ **stat**(`uri`): [`Thenable`](Thenable.md)<[`FileStat`](codearts_plugin_.FileStat.md)\>

Retrieve metadata about a file.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The uri of the file to retrieve metadata about. |

#### Returns

[`Thenable`](Thenable.md)<[`FileStat`](codearts_plugin_.FileStat.md)\>

The file metadata about the file.

#### Defined in

[index.d.ts:8098](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8098)

___

### writeFile

▸ **writeFile**(`uri`, `content`): [`Thenable`](Thenable.md)<`void`\>

Write data to a file, replacing its entire contents.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The uri of the file. |
| `content` | `Uint8Array` | The new content of the file. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8132](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8132)
