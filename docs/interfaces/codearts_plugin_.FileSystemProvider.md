[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileSystemProvider

# Interface: FileSystemProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileSystemProvider

The filesystem provider defines what the editor needs to read, write, discover,
and to manage files and folders. It allows extensions to serve files from remote places,
like ftp-servers, and to seamlessly integrate those into the editor.

* *Note 1:* The filesystem provider API works with [uris](../classes/codearts_plugin_.Uri.md) and assumes hierarchical
paths, e.g. `foo:/my/path` is a child of `foo:/my/` and a parent of `foo:/my/path/deeper`.
* *Note 2:* There is an activation event `onFileSystem:<scheme>` that fires when a file
or folder is being accessed.
* *Note 3:* The word 'file' is often used to denote all [kinds](../enums/codearts_plugin_.FileType.md) of files, e.g.
folders, symbolic links, and regular files.

## Table of contents

### Properties

- [onDidChangeFile](codearts_plugin_.FileSystemProvider.md#ondidchangefile)

### Methods

- [copy](codearts_plugin_.FileSystemProvider.md#copy)
- [createDirectory](codearts_plugin_.FileSystemProvider.md#createdirectory)
- [delete](codearts_plugin_.FileSystemProvider.md#delete)
- [readDirectory](codearts_plugin_.FileSystemProvider.md#readdirectory)
- [readFile](codearts_plugin_.FileSystemProvider.md#readfile)
- [rename](codearts_plugin_.FileSystemProvider.md#rename)
- [stat](codearts_plugin_.FileSystemProvider.md#stat)
- [watch](codearts_plugin_.FileSystemProvider.md#watch)
- [writeFile](codearts_plugin_.FileSystemProvider.md#writefile)

## Properties

### onDidChangeFile

• `Readonly` **onDidChangeFile**: [`Event`](codearts_plugin_.Event.md)<[`FileChangeEvent`](codearts_plugin_.FileChangeEvent.md)[]\>

An event to signal that a resource has been created, changed, or deleted. This
event should fire for resources that are being [watched](codearts_plugin_.FileSystemProvider.md#watch)
by clients of this provider.

*Note:* It is important that the metadata of the file that changed provides an
updated `mtime` that advanced from the previous value in the [stat](codearts_plugin_.FileStat.md) and a
correct `size` value. Otherwise there may be optimizations in place that will not show
the change in an editor for example.

#### Defined in

[index.d.ts:8025](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8025)

## Methods

### copy

▸ `Optional` **copy**(`source`, `destination`, `options`): `void` \| [`Thenable`](Thenable.md)<`void`\>

Copy files or folders. Implementing this function is optional but it will speedup
the copy operation.

**`Throws`**

[`FileNotFound`](../classes/codearts_plugin_.FileSystemError.md#filenotfound) when `source` doesn't exist.

**`Throws`**

[`FileNotFound`](../classes/codearts_plugin_.FileSystemError.md#filenotfound) when parent of `destination` doesn't exist, e.g. no mkdirp-logic required.

**`Throws`**

[`FileExists`](../classes/codearts_plugin_.FileSystemError.md#fileexists) when `destination` exists and when the `overwrite` option is not `true`.

**`Throws`**

[`NoPermissions`](../classes/codearts_plugin_.FileSystemError.md#nopermissions) when permissions aren't sufficient.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The existing file. |
| `destination` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The destination location. |
| `options` | `Object` | Defines if existing files should be overwritten. |
| `options.overwrite` | `boolean` | - |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8139](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8139)

___

### createDirectory

▸ **createDirectory**(`uri`): `void` \| [`Thenable`](Thenable.md)<`void`\>

Create a new directory (Note, that new files are created via `write`-calls).

**`Throws`**

[`FileNotFound`](../classes/codearts_plugin_.FileSystemError.md#filenotfound) when the parent of `uri` doesn't exist, e.g. no mkdirp-logic required.

**`Throws`**

[`FileExists`](../classes/codearts_plugin_.FileSystemError.md#fileexists) when `uri` already exists.

**`Throws`**

[`NoPermissions`](../classes/codearts_plugin_.FileSystemError.md#nopermissions) when permissions aren't sufficient.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The uri of the new folder. |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8080](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8080)

___

### delete

▸ **delete**(`uri`, `options`): `void` \| [`Thenable`](Thenable.md)<`void`\>

Delete a file.

**`Throws`**

[`FileNotFound`](../classes/codearts_plugin_.FileSystemError.md#filenotfound) when `uri` doesn't exist.

**`Throws`**

[`NoPermissions`](../classes/codearts_plugin_.FileSystemError.md#nopermissions) when permissions aren't sufficient.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The resource that is to be deleted. |
| `options` | `Object` | Defines if deletion of folders is recursive. |
| `options.recursive` | `boolean` | - |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8112](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8112)

___

### readDirectory

▸ **readDirectory**(`uri`): [`string`, [`FileType`](../enums/codearts_plugin_.FileType.md)][] \| [`Thenable`](Thenable.md)<[`string`, [`FileType`](../enums/codearts_plugin_.FileType.md)][]\>

Retrieve all entries of a [directory](../enums/codearts_plugin_.FileType.md#directory).

**`Throws`**

[`FileNotFound`](../classes/codearts_plugin_.FileSystemError.md#filenotfound) when `uri` doesn't exist.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The uri of the folder. |

#### Returns

[`string`, [`FileType`](../enums/codearts_plugin_.FileType.md)][] \| [`Thenable`](Thenable.md)<[`string`, [`FileType`](../enums/codearts_plugin_.FileType.md)][]\>

An array of name/type-tuples or a thenable that resolves to such.

#### Defined in

[index.d.ts:8070](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8070)

___

### readFile

▸ **readFile**(`uri`): `Uint8Array` \| [`Thenable`](Thenable.md)<`Uint8Array`\>

Read the entire contents of a file.

**`Throws`**

[`FileNotFound`](../classes/codearts_plugin_.FileSystemError.md#filenotfound) when `uri` doesn't exist.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The uri of the file. |

#### Returns

`Uint8Array` \| [`Thenable`](Thenable.md)<`Uint8Array`\>

An array of bytes or a thenable that resolves to such.

#### Defined in

[index.d.ts:8089](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8089)

___

### rename

▸ **rename**(`oldUri`, `newUri`, `options`): `void` \| [`Thenable`](Thenable.md)<`void`\>

Rename a file or folder.

**`Throws`**

[`FileNotFound`](../classes/codearts_plugin_.FileSystemError.md#filenotfound) when `oldUri` doesn't exist.

**`Throws`**

[`FileNotFound`](../classes/codearts_plugin_.FileSystemError.md#filenotfound) when parent of `newUri` doesn't exist, e.g. no mkdirp-logic required.

**`Throws`**

[`FileExists`](../classes/codearts_plugin_.FileSystemError.md#fileexists) when `newUri` exists and when the `overwrite` option is not `true`.

**`Throws`**

[`NoPermissions`](../classes/codearts_plugin_.FileSystemError.md#nopermissions) when permissions aren't sufficient.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldUri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The existing file. |
| `newUri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The new location. |
| `options` | `Object` | Defines if existing files should be overwritten. |
| `options.overwrite` | `boolean` | - |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8125](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8125)

___

### stat

▸ **stat**(`uri`): [`FileStat`](codearts_plugin_.FileStat.md) \| [`Thenable`](Thenable.md)<[`FileStat`](codearts_plugin_.FileStat.md)\>

Retrieve metadata about a file.

Note that the metadata for symbolic links should be the metadata of the file they refer to.
Still, the [SymbolicLink](../enums/codearts_plugin_.FileType.md#symboliclink)-type must be used in addition to the actual type, e.g.
`FileType.SymbolicLink | FileType.Directory`.

**`Throws`**

[`FileNotFound`](../classes/codearts_plugin_.FileSystemError.md#filenotfound) when `uri` doesn't exist.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The uri of the file to retrieve metadata about. |

#### Returns

[`FileStat`](codearts_plugin_.FileStat.md) \| [`Thenable`](Thenable.md)<[`FileStat`](codearts_plugin_.FileStat.md)\>

The file metadata about the file.

#### Defined in

[index.d.ts:8061](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8061)

___

### watch

▸ **watch**(`uri`, `options`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Subscribes to file change events in the file or folder denoted by `uri`. For folders,
the option `recursive` indicates whether subfolders, sub-subfolders, etc. should
be watched for file changes as well. With `recursive: false`, only changes to the
files that are direct children of the folder should trigger an event.

The `excludes` array is used to indicate paths that should be excluded from file
watching. It is typically derived from the `files.watcherExclude` setting that
is configurable by the user. Each entry can be be:
- the absolute path to exclude
- a relative path to exclude (for example `build/output`)
- a simple glob pattern (for example `**​/build`, `output/**`)

It is the file system provider's job to call [`onDidChangeFile`](codearts_plugin_.FileSystemProvider.md#ondidchangefile)
for every change given these rules. No event should be emitted for files that match any of the provided
excludes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The uri of the file or folder to be watched. |
| `options` | `Object` | Configures the watch. |
| `options.excludes` | readonly `string`[] | - |
| `options.recursive` | `boolean` | - |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable that tells the provider to stop watching the `uri`.

#### Defined in

[index.d.ts:8048](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8048)

___

### writeFile

▸ **writeFile**(`uri`, `content`, `options`): `void` \| [`Thenable`](Thenable.md)<`void`\>

Write data to a file, replacing its entire contents.

**`Throws`**

[`FileNotFound`](../classes/codearts_plugin_.FileSystemError.md#filenotfound) when `uri` doesn't exist and `create` is not set.

**`Throws`**

[`FileNotFound`](../classes/codearts_plugin_.FileSystemError.md#filenotfound) when the parent of `uri` doesn't exist and `create` is set, e.g. no mkdirp-logic required.

**`Throws`**

[`FileExists`](../classes/codearts_plugin_.FileSystemError.md#fileexists) when `uri` already exists, `create` is set but `overwrite` is not set.

**`Throws`**

[`NoPermissions`](../classes/codearts_plugin_.FileSystemError.md#nopermissions) when permissions aren't sufficient.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The uri of the file. |
| `content` | `Uint8Array` | The new content of the file. |
| `options` | `Object` | Defines if missing files should or must be created. |
| `options.create` | `boolean` | - |
| `options.overwrite` | `boolean` | - |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8102](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8102)
