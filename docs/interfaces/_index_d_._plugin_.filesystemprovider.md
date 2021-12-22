**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FileSystemProvider

# Interface: FileSystemProvider

The filesystem provider defines what the editor needs to read, write, discover,
and to manage files and folders. It allows extensions to serve files from remote places,
like ftp-servers, and to seamlessly integrate those into the editor.

* *Note 1:* The filesystem provider API works with [uris](#Uri) and assumes hierarchical
paths, e.g. `foo:/my/path` is a child of `foo:/my/` and a parent of `foo:/my/path/deeper`.
* *Note 2:* There is an activation event `onFileSystem:<scheme>` that fires when a file
or folder is being accessed.
* *Note 3:* The word 'file' is often used to denote all [kinds](#FileType) of files, e.g.
folders, symbolic links, and regular files.

## Hierarchy

* **FileSystemProvider**

## Index

### Properties

* [onDidChangeFile](_index_d_._plugin_.filesystemprovider.md#ondidchangefile)

### Methods

* [copy](_index_d_._plugin_.filesystemprovider.md#copy)
* [createDirectory](_index_d_._plugin_.filesystemprovider.md#createdirectory)
* [delete](_index_d_._plugin_.filesystemprovider.md#delete)
* [readDirectory](_index_d_._plugin_.filesystemprovider.md#readdirectory)
* [readFile](_index_d_._plugin_.filesystemprovider.md#readfile)
* [rename](_index_d_._plugin_.filesystemprovider.md#rename)
* [stat](_index_d_._plugin_.filesystemprovider.md#stat)
* [watch](_index_d_._plugin_.filesystemprovider.md#watch)
* [writeFile](_index_d_._plugin_.filesystemprovider.md#writefile)

## Properties

### onDidChangeFile

• `Readonly` **onDidChangeFile**: [Event](_index_d_._plugin_.event.md)\<[FileChangeEvent](_index_d_._plugin_.filechangeevent.md)[]>

*Defined in [index.d.ts:7007](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7007)*

An event to signal that a resource has been created, changed, or deleted. This
event should fire for resources that are being [watched](#FileSystemProvider.watch)
by clients of this provider.

*Note:* It is important that the metadata of the file that changed provides an
updated `mtime` that advanced from the previous value in the [stat](#FileStat) and a
correct `size` value. Otherwise there may be optimizations in place that will not show
the change in an editor for example.

## Methods

### copy

▸ `Optional`**copy**(`source`: [Uri](../classes/_index_d_._plugin_.uri.md), `destination`: [Uri](../classes/_index_d_._plugin_.uri.md), `options`: { overwrite: boolean  }): void \| [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:7111](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7111)*

Copy files or folders. Implementing this function is optional but it will speedup
the copy operation.

**`throws`** [`FileNotFound`](#FileSystemError.FileNotFound) when `source` doesn't exist.

**`throws`** [`FileNotFound`](#FileSystemError.FileNotFound) when parent of `destination` doesn't exist, e.g. no mkdirp-logic required.

**`throws`** [`FileExists`](#FileSystemError.FileExists) when `destination` exists and when the `overwrite` option is not `true`.

**`throws`** [`NoPermissions`](#FileSystemError.NoPermissions) when permissions aren't sufficient.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`source` | [Uri](../classes/_index_d_._plugin_.uri.md) | The existing file. |
`destination` | [Uri](../classes/_index_d_._plugin_.uri.md) | The destination location. |
`options` | { overwrite: boolean  } | Defines if existing files should be overwritten. |

**Returns:** void \| [Thenable](_index_d_.thenable.md)\<void>

___

### createDirectory

▸ **createDirectory**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md)): void \| [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:7052](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7052)*

Create a new directory (Note, that new files are created via `write`-calls).

**`throws`** [`FileNotFound`](#FileSystemError.FileNotFound) when the parent of `uri` doesn't exist, e.g. no mkdirp-logic required.

**`throws`** [`FileExists`](#FileSystemError.FileExists) when `uri` already exists.

**`throws`** [`NoPermissions`](#FileSystemError.NoPermissions) when permissions aren't sufficient.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the new folder. |

**Returns:** void \| [Thenable](_index_d_.thenable.md)\<void>

___

### delete

▸ **delete**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md), `options`: { recursive: boolean  }): void \| [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:7084](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7084)*

Delete a file.

**`throws`** [`FileNotFound`](#FileSystemError.FileNotFound) when `uri` doesn't exist.

**`throws`** [`NoPermissions`](#FileSystemError.NoPermissions) when permissions aren't sufficient.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The resource that is to be deleted. |
`options` | { recursive: boolean  } | Defines if deletion of folders is recursive. |

**Returns:** void \| [Thenable](_index_d_.thenable.md)\<void>

___

### readDirectory

▸ **readDirectory**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md)): [string, [FileType](../enums/_index_d_._plugin_.filetype.md)][] \| [Thenable](_index_d_.thenable.md)\<[string, [FileType](../enums/_index_d_._plugin_.filetype.md)][]>

*Defined in [index.d.ts:7042](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7042)*

Retrieve all entries of a [directory](#FileType.Directory).

**`throws`** [`FileNotFound`](#FileSystemError.FileNotFound) when `uri` doesn't exist.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the folder. |

**Returns:** [string, [FileType](../enums/_index_d_._plugin_.filetype.md)][] \| [Thenable](_index_d_.thenable.md)\<[string, [FileType](../enums/_index_d_._plugin_.filetype.md)][]>

An array of name/type-tuples or a thenable that resolves to such.

___

### readFile

▸ **readFile**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md)): Uint8Array \| [Thenable](_index_d_.thenable.md)\<Uint8Array>

*Defined in [index.d.ts:7061](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7061)*

Read the entire contents of a file.

**`throws`** [`FileNotFound`](#FileSystemError.FileNotFound) when `uri` doesn't exist.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the file. |

**Returns:** Uint8Array \| [Thenable](_index_d_.thenable.md)\<Uint8Array>

An array of bytes or a thenable that resolves to such.

___

### rename

▸ **rename**(`oldUri`: [Uri](../classes/_index_d_._plugin_.uri.md), `newUri`: [Uri](../classes/_index_d_._plugin_.uri.md), `options`: { overwrite: boolean  }): void \| [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:7097](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7097)*

Rename a file or folder.

**`throws`** [`FileNotFound`](#FileSystemError.FileNotFound) when `oldUri` doesn't exist.

**`throws`** [`FileNotFound`](#FileSystemError.FileNotFound) when parent of `newUri` doesn't exist, e.g. no mkdirp-logic required.

**`throws`** [`FileExists`](#FileSystemError.FileExists) when `newUri` exists and when the `overwrite` option is not `true`.

**`throws`** [`NoPermissions`](#FileSystemError.NoPermissions) when permissions aren't sufficient.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`oldUri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The existing file. |
`newUri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The new location. |
`options` | { overwrite: boolean  } | Defines if existing files should be overwritten. |

**Returns:** void \| [Thenable](_index_d_.thenable.md)\<void>

___

### stat

▸ **stat**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md)): [FileStat](_index_d_._plugin_.filestat.md) \| [Thenable](_index_d_.thenable.md)\<[FileStat](_index_d_._plugin_.filestat.md)>

*Defined in [index.d.ts:7033](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7033)*

Retrieve metadata about a file.

Note that the metadata for symbolic links should be the metadata of the file they refer to.
Still, the [SymbolicLink](#FileType.SymbolicLink)-type must be used in addition to the actual type, e.g.
`FileType.SymbolicLink | FileType.Directory`.

**`throws`** [`FileNotFound`](#FileSystemError.FileNotFound) when `uri` doesn't exist.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the file to retrieve metadata about. |

**Returns:** [FileStat](_index_d_._plugin_.filestat.md) \| [Thenable](_index_d_.thenable.md)\<[FileStat](_index_d_._plugin_.filestat.md)>

The file metadata about the file.

___

### watch

▸ **watch**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md), `options`: { excludes: string[] ; recursive: boolean  }): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:7020](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7020)*

Subscribe to events in the file or folder denoted by `uri`.

The editor will call this function for files and folders. In the latter case, the
options differ from defaults, e.g. what files/folders to exclude from watching
and if subfolders, sub-subfolder, etc. should be watched (`recursive`).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the file to be watched. |
`options` | { excludes: string[] ; recursive: boolean  } | Configures the watch. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A disposable that tells the provider to stop watching the `uri`.

___

### writeFile

▸ **writeFile**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md), `content`: Uint8Array, `options`: { create: boolean ; overwrite: boolean  }): void \| [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:7074](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7074)*

Write data to a file, replacing its entire contents.

**`throws`** [`FileNotFound`](#FileSystemError.FileNotFound) when `uri` doesn't exist and `create` is not set.

**`throws`** [`FileNotFound`](#FileSystemError.FileNotFound) when the parent of `uri` doesn't exist and `create` is set, e.g. no mkdirp-logic required.

**`throws`** [`FileExists`](#FileSystemError.FileExists) when `uri` already exists, `create` is set but `overwrite` is not set.

**`throws`** [`NoPermissions`](#FileSystemError.NoPermissions) when permissions aren't sufficient.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the file. |
`content` | Uint8Array | The new content of the file. |
`options` | { create: boolean ; overwrite: boolean  } | Defines if missing files should or must be created. |

**Returns:** void \| [Thenable](_index_d_.thenable.md)\<void>
