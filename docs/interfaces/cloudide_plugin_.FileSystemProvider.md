[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / FileSystemProvider

# Interface: FileSystemProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).FileSystemProvider

The filesystem provider defines what the editor needs to read, write, discover,
and to manage files and folders. It allows extensions to serve files from remote places,
like ftp-servers, and to seamlessly integrate those into the editor.

* *Note 1:* The filesystem provider API works with [uris](#Uri) and assumes hierarchical
paths, e.g. `foo:/my/path` is a child of `foo:/my/` and a parent of `foo:/my/path/deeper`.
* *Note 2:* There is an activation event `onFileSystem:<scheme>` that fires when a file
or folder is being accessed.
* *Note 3:* The word 'file' is often used to denote all [kinds](#FileType) of files, e.g.
folders, symbolic links, and regular files.

## Table of contents

### Properties

- [onDidChangeFile](cloudide_plugin_.FileSystemProvider.md#ondidchangefile)

### Methods

- [copy](cloudide_plugin_.FileSystemProvider.md#copy)
- [createDirectory](cloudide_plugin_.FileSystemProvider.md#createdirectory)
- [delete](cloudide_plugin_.FileSystemProvider.md#delete)
- [readDirectory](cloudide_plugin_.FileSystemProvider.md#readdirectory)
- [readFile](cloudide_plugin_.FileSystemProvider.md#readfile)
- [rename](cloudide_plugin_.FileSystemProvider.md#rename)
- [stat](cloudide_plugin_.FileSystemProvider.md#stat)
- [watch](cloudide_plugin_.FileSystemProvider.md#watch)
- [writeFile](cloudide_plugin_.FileSystemProvider.md#writefile)

## Properties

### onDidChangeFile

• `Readonly` **onDidChangeFile**: [`Event`](cloudide_plugin_.Event.md)<[`FileChangeEvent`](cloudide_plugin_.FileChangeEvent.md)[]\>

An event to signal that a resource has been created, changed, or deleted. This
event should fire for resources that are being [watched](#FileSystemProvider.watch)
by clients of this provider.

*Note:* It is important that the metadata of the file that changed provides an
updated `mtime` that advanced from the previous value in the [stat](#FileStat) and a
correct `size` value. Otherwise there may be optimizations in place that will not show
the change in an editor for example.

#### Defined in

[index.d.ts:5774](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5774)

## Methods

### copy

▸ `Optional` **copy**(`source`, `destination`, `options`): `void` \| `Promise`<`void`\>

Copy files or folders. Implementing this function is optional but it will speedup
the copy operation.

**`Throws`**

[`FileNotFound`](#FileSystemError.FileNotFound) when `source` doesn't exist.

**`Throws`**

[`FileNotFound`](#FileSystemError.FileNotFound) when parent of `destination` doesn't exist, e.g. no mkdirp-logic required.

**`Throws`**

[`FileExists`](#FileSystemError.FileExists) when `destination` exists and when the `overwrite` option is not `true`.

**`Throws`**

[`NoPermissions`](#FileSystemError.NoPermissions) when permissions aren't sufficient.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The existing file. |
| `destination` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The destination location. |
| `options` | `Object` | Defines if existing files should be overwritten. |
| `options.overwrite` | `boolean` | - |

#### Returns

`void` \| `Promise`<`void`\>

#### Defined in

[index.d.ts:5878](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5878)

___

### createDirectory

▸ **createDirectory**(`uri`): `void` \| `Promise`<`void`\>

Create a new directory (Note, that new files are created via `write`-calls).

**`Throws`**

[`FileNotFound`](#FileSystemError.FileNotFound) when the parent of `uri` doesn't exist, e.g. no mkdirp-logic required.

**`Throws`**

[`FileExists`](#FileSystemError.FileExists) when `uri` already exists.

**`Throws`**

[`NoPermissions`](#FileSystemError.NoPermissions) when permissions aren't sufficient.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The uri of the new folder. |

#### Returns

`void` \| `Promise`<`void`\>

#### Defined in

[index.d.ts:5819](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5819)

___

### delete

▸ **delete**(`uri`, `options`): `void` \| `Promise`<`void`\>

Delete a file.

**`Throws`**

[`FileNotFound`](#FileSystemError.FileNotFound) when `uri` doesn't exist.

**`Throws`**

[`NoPermissions`](#FileSystemError.NoPermissions) when permissions aren't sufficient.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The resource that is to be deleted. |
| `options` | `Object` | Defines if deletion of folders is recursive. |
| `options.recursive` | `boolean` | - |

#### Returns

`void` \| `Promise`<`void`\>

#### Defined in

[index.d.ts:5851](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5851)

___

### readDirectory

▸ **readDirectory**(`uri`): [`string`, [`FileType`](../enums/cloudide_plugin_.FileType.md)][] \| `Promise`<[`string`, [`FileType`](../enums/cloudide_plugin_.FileType.md)][]\>

Retrieve all entries of a [directory](#FileType.Directory).

**`Throws`**

[`FileNotFound`](#FileSystemError.FileNotFound) when `uri` doesn't exist.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The uri of the folder. |

#### Returns

[`string`, [`FileType`](../enums/cloudide_plugin_.FileType.md)][] \| `Promise`<[`string`, [`FileType`](../enums/cloudide_plugin_.FileType.md)][]\>

An array of name/type-tuples or a thenable that resolves to such.

#### Defined in

[index.d.ts:5809](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5809)

___

### readFile

▸ **readFile**(`uri`): `Uint8Array` \| `Promise`<`Uint8Array`\>

Read the entire contents of a file.

**`Throws`**

[`FileNotFound`](#FileSystemError.FileNotFound) when `uri` doesn't exist.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The uri of the file. |

#### Returns

`Uint8Array` \| `Promise`<`Uint8Array`\>

An array of bytes or a thenable that resolves to such.

#### Defined in

[index.d.ts:5828](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5828)

___

### rename

▸ **rename**(`oldUri`, `newUri`, `options`): `void` \| `Promise`<`void`\>

Rename a file or folder.

**`Throws`**

[`FileNotFound`](#FileSystemError.FileNotFound) when `oldUri` doesn't exist.

**`Throws`**

[`FileNotFound`](#FileSystemError.FileNotFound) when parent of `newUri` doesn't exist, e.g. no mkdirp-logic required.

**`Throws`**

[`FileExists`](#FileSystemError.FileExists) when `newUri` exists and when the `overwrite` option is not `true`.

**`Throws`**

[`NoPermissions`](#FileSystemError.NoPermissions) when permissions aren't sufficient.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldUri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The existing file. |
| `newUri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The new location. |
| `options` | `Object` | Defines if existing files should be overwritten. |
| `options.overwrite` | `boolean` | - |

#### Returns

`void` \| `Promise`<`void`\>

#### Defined in

[index.d.ts:5864](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5864)

___

### stat

▸ **stat**(`uri`): [`FileStat`](cloudide_plugin_.FileStat.md) \| `Promise`<[`FileStat`](cloudide_plugin_.FileStat.md)\>

Retrieve metadata about a file.

Note that the metadata for symbolic links should be the metadata of the file they refer to.
Still, the [SymbolicLink](#FileType.SymbolicLink)-type must be used in addition to the actual type, e.g.
`FileType.SymbolicLink | FileType.Directory`.

**`Throws`**

[`FileNotFound`](#FileSystemError.FileNotFound) when `uri` doesn't exist.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The uri of the file to retrieve metadata about. |

#### Returns

[`FileStat`](cloudide_plugin_.FileStat.md) \| `Promise`<[`FileStat`](cloudide_plugin_.FileStat.md)\>

The file metadata about the file.

#### Defined in

[index.d.ts:5800](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5800)

___

### watch

▸ **watch**(`uri`, `options`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Subscribe to events in the file or folder denoted by `uri`.

The editor will call this function for files and folders. In the latter case, the
options differ from defaults, e.g. what files/folders to exclude from watching
and if subfolders, sub-subfolder, etc. should be watched (`recursive`).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The uri of the file to be watched. |
| `options` | `Object` | Configures the watch. |
| `options.excludes` | `string`[] | - |
| `options.recursive` | `boolean` | - |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A disposable that tells the provider to stop watching the `uri`.

#### Defined in

[index.d.ts:5787](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5787)

___

### writeFile

▸ **writeFile**(`uri`, `content`, `options`): `void` \| `Promise`<`void`\>

Write data to a file, replacing its entire contents.

**`Throws`**

[`FileNotFound`](#FileSystemError.FileNotFound) when `uri` doesn't exist and `create` is not set.

**`Throws`**

[`FileNotFound`](#FileSystemError.FileNotFound) when the parent of `uri` doesn't exist and `create` is set, e.g. no mkdirp-logic required.

**`Throws`**

[`FileExists`](#FileSystemError.FileExists) when `uri` already exists, `create` is set but `overwrite` is not set.

**`Throws`**

[`NoPermissions`](#FileSystemError.NoPermissions) when permissions aren't sufficient.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The uri of the file. |
| `content` | `Uint8Array` | The new content of the file. |
| `options` | `Object` | Defines if missing files should or must be created. |
| `options.create` | `boolean` | - |
| `options.overwrite` | `boolean` | - |

#### Returns

`void` \| `Promise`<`void`\>

#### Defined in

[index.d.ts:5841](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5841)
