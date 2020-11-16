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
* [readDirectory](_index_d_._plugin_.filesystem.md#readdirectory)
* [readFile](_index_d_._plugin_.filesystem.md#readfile)
* [rename](_index_d_._plugin_.filesystem.md#rename)
* [stat](_index_d_._plugin_.filesystem.md#stat)
* [writeFile](_index_d_._plugin_.filesystem.md#writefile)

## Methods

### copy

▸ **copy**(`source`: [Uri](../classes/_index_d_._plugin_.uri.md), `target`: [Uri](../classes/_index_d_._plugin_.uri.md), `options?`: { overwrite?: boolean  }): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:6578](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6578)*

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

*Defined in [index.d.ts:6536](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6536)*

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

*Defined in [index.d.ts:6560](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6560)*

Delete a file.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The resource that is to be deleted. |
`options?` | { recursive?: boolean ; useTrash?: boolean  } | Defines if trash can should be used and if deletion of folders is recursive  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>

___

### readDirectory

▸ **readDirectory**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md)): [Thenable](_index_d_.thenable.md)\<[string, [FileType](../enums/_index_d_._plugin_.filetype.md)][]>

*Defined in [index.d.ts:6526](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6526)*

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

*Defined in [index.d.ts:6544](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6544)*

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

*Defined in [index.d.ts:6569](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6569)*

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

*Defined in [index.d.ts:6518](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6518)*

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

*Defined in [index.d.ts:6552](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6552)*

Write data to a file, replacing its entire contents.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the file. |
`content` | Uint8Array | The new content of the file.  |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>
