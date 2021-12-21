**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FileSystem

# Interface: FileSystem

The file system interface exposes the editor's built-in and contributed
[file system providers](#FileSystemProvider). It allows extensions to work
with files from the local disk as well as files from remote places, like the
remote extension host or ftp-servers.

*Note* that an instance of this interface is available as [`workspace.fs`](#workspace.fs).

## Hierarchy

* **FileSystem**

## Index

### Methods

* [copy](_index_d_._plugin_.filesystem.md#copy)
* [createDirectory](_index_d_._plugin_.filesystem.md#createdirectory)
* [delete](_index_d_._plugin_.filesystem.md#delete)
* [isWritableFileSystem](_index_d_._plugin_.filesystem.md#iswritablefilesystem)
* [readDirectory](_index_d_._plugin_.filesystem.md#readdirectory)
* [readFile](_index_d_._plugin_.filesystem.md#readfile)
* [rename](_index_d_._plugin_.filesystem.md#rename)
* [stat](_index_d_._plugin_.filesystem.md#stat)
* [writeFile](_index_d_._plugin_.filesystem.md#writefile)

## Methods

### copy

▸ **copy**(`source`: [Uri](../classes/_index_d_._plugin_.uri.md), `target`: [Uri](../classes/_index_d_._plugin_.uri.md), `options?`: { overwrite?: boolean  }): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:7187](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7187)*

Copy files or folders.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`source` | [Uri](../classes/_index_d_._plugin_.uri.md) | The existing file. |
`target` | [Uri](../classes/_index_d_._plugin_.uri.md) | - |
`options?` | { overwrite?: boolean  } | Defines if existing files should be overwritten.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>

___

### createDirectory

▸ **createDirectory**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md)): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:7145](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7145)*

Create a new directory (Note, that new files are created via `write`-calls).

*Note* that missing directories are created automatically, e.g this call has
`mkdirp` semantics.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the new folder.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>

___

### delete

▸ **delete**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md), `options?`: { recursive?: boolean ; useTrash?: boolean  }): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:7169](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7169)*

Delete a file.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The resource that is to be deleted. |
`options?` | { recursive?: boolean ; useTrash?: boolean  } | Defines if trash can should be used and if deletion of folders is recursive  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>

___

### isWritableFileSystem

▸ **isWritableFileSystem**(`scheme`: string): boolean \| undefined

*Defined in [index.d.ts:7202](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7202)*

Check if a given file system supports writing files.

Keep in mind that just because a file system supports writing, that does
not mean that writes will always succeed. There may be permissions issues
or other errors that prevent writing a file.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`scheme` | string | The scheme of the filesystem, for example `file` or `git`.  |

**Returns:** boolean \| undefined

`true` if the file system supports writing, `false` if it does not
support writing (i.e. it is readonly), and `undefined` if VS Code does not
know about the filesystem.

___

### readDirectory

▸ **readDirectory**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md)): [Thenable](_index_d_.thenable.md)\<[string, [FileType](../enums/_index_d_._plugin_.filetype.md)][]>

*Defined in [index.d.ts:7135](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7135)*

Retrieve all entries of a [directory](#FileType.Directory).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the folder. |

**Returns:** [Thenable](_index_d_.thenable.md)\<[string, [FileType](../enums/_index_d_._plugin_.filetype.md)][]>

An array of name/type-tuples or a thenable that resolves to such.

___

### readFile

▸ **readFile**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md)): [Thenable](_index_d_.thenable.md)\<Uint8Array>

*Defined in [index.d.ts:7153](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7153)*

Read the entire contents of a file.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the file. |

**Returns:** [Thenable](_index_d_.thenable.md)\<Uint8Array>

An array of bytes or a thenable that resolves to such.

___

### rename

▸ **rename**(`source`: [Uri](../classes/_index_d_._plugin_.uri.md), `target`: [Uri](../classes/_index_d_._plugin_.uri.md), `options?`: { overwrite?: boolean  }): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:7178](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7178)*

Rename a file or folder.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`source` | [Uri](../classes/_index_d_._plugin_.uri.md) | - |
`target` | [Uri](../classes/_index_d_._plugin_.uri.md) | - |
`options?` | { overwrite?: boolean  } | Defines if existing files should be overwritten.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>

___

### stat

▸ **stat**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md)): [Thenable](_index_d_.thenable.md)\<[FileStat](_index_d_._plugin_.filestat.md)>

*Defined in [index.d.ts:7127](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7127)*

Retrieve metadata about a file.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the file to retrieve metadata about. |

**Returns:** [Thenable](_index_d_.thenable.md)\<[FileStat](_index_d_._plugin_.filestat.md)>

The file metadata about the file.

___

### writeFile

▸ **writeFile**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md), `content`: Uint8Array): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:7161](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7161)*

Write data to a file, replacing its entire contents.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the file. |
`content` | Uint8Array | The new content of the file.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>
