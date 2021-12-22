**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / WorkspaceEdit

# Class: WorkspaceEdit

A workspace edit is a collection of textual and files changes for
multiple resources and documents.

Use the [applyEdit](#workspace.applyEdit)-function to apply a workspace edit.

## Hierarchy

* **WorkspaceEdit**

## Index

### Properties

* [size](_index_d_._plugin_.workspaceedit.md#size)

### Methods

* [createFile](_index_d_._plugin_.workspaceedit.md#createfile)
* [delete](_index_d_._plugin_.workspaceedit.md#delete)
* [deleteFile](_index_d_._plugin_.workspaceedit.md#deletefile)
* [entries](_index_d_._plugin_.workspaceedit.md#entries)
* [get](_index_d_._plugin_.workspaceedit.md#get)
* [has](_index_d_._plugin_.workspaceedit.md#has)
* [insert](_index_d_._plugin_.workspaceedit.md#insert)
* [renameFile](_index_d_._plugin_.workspaceedit.md#renamefile)
* [replace](_index_d_._plugin_.workspaceedit.md#replace)
* [set](_index_d_._plugin_.workspaceedit.md#set)

## Properties

### size

• `Readonly` **size**: number

*Defined in [index.d.ts:3211](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3211)*

The number of affected resources of textual or resource changes.

## Methods

### createFile

▸ **createFile**(`uri`: [Uri](_index_d_._plugin_.uri.md), `options?`: { ignoreIfExists?: boolean ; overwrite?: boolean  }, `metadata?`: [WorkspaceEditEntryMetadata](../interfaces/_index_d_._plugin_.workspaceeditentrymetadata.md)): void

*Defined in [index.d.ts:3276](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3276)*

Create a regular file.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](_index_d_._plugin_.uri.md) | Uri of the new file.. |
`options?` | { ignoreIfExists?: boolean ; overwrite?: boolean  } | Defines if an existing file should be overwritten or be ignored. When overwrite and ignoreIfExists are both set overwrite wins. When both are unset and when the file already exists then the edit cannot be applied successfully. |
`metadata?` | [WorkspaceEditEntryMetadata](../interfaces/_index_d_._plugin_.workspaceeditentrymetadata.md) | Optional metadata for the entry.  |

**Returns:** void

___

### delete

▸ **delete**(`uri`: [Uri](_index_d_._plugin_.uri.md), `range`: [Range](_index_d_._plugin_.range.md), `metadata?`: [WorkspaceEditEntryMetadata](../interfaces/_index_d_._plugin_.workspaceeditentrymetadata.md)): void

*Defined in [index.d.ts:3240](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3240)*

Delete the text at the given range.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](_index_d_._plugin_.uri.md) | A resource identifier. |
`range` | [Range](_index_d_._plugin_.range.md) | A range. |
`metadata?` | [WorkspaceEditEntryMetadata](../interfaces/_index_d_._plugin_.workspaceeditentrymetadata.md) | Optional metadata for the entry.  |

**Returns:** void

___

### deleteFile

▸ **deleteFile**(`uri`: [Uri](_index_d_._plugin_.uri.md), `options?`: { ignoreIfNotExists?: boolean ; recursive?: boolean  }, `metadata?`: [WorkspaceEditEntryMetadata](../interfaces/_index_d_._plugin_.workspaceeditentrymetadata.md)): void

*Defined in [index.d.ts:3284](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3284)*

Delete a file or folder.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](_index_d_._plugin_.uri.md) | The uri of the file that is to be deleted. |
`options?` | { ignoreIfNotExists?: boolean ; recursive?: boolean  } | - |
`metadata?` | [WorkspaceEditEntryMetadata](../interfaces/_index_d_._plugin_.workspaceeditentrymetadata.md) | Optional metadata for the entry.  |

**Returns:** void

___

### entries

▸ **entries**(): [[Uri](_index_d_._plugin_.uri.md), [TextEdit](_index_d_._plugin_.textedit.md)[]][]

*Defined in [index.d.ts:3302](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3302)*

Get all text edits grouped by resource.

**Returns:** [[Uri](_index_d_._plugin_.uri.md), [TextEdit](_index_d_._plugin_.textedit.md)[]][]

A shallow copy of `[Uri, TextEdit[]]`-tuples.

___

### get

▸ **get**(`uri`: [Uri](_index_d_._plugin_.uri.md)): [TextEdit](_index_d_._plugin_.textedit.md)[]

*Defined in [index.d.ts:3264](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3264)*

Get the text edits for a resource.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](_index_d_._plugin_.uri.md) | A resource identifier. |

**Returns:** [TextEdit](_index_d_._plugin_.textedit.md)[]

An array of text edits.

___

### has

▸ **has**(`uri`: [Uri](_index_d_._plugin_.uri.md)): boolean

*Defined in [index.d.ts:3248](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3248)*

Check if a text edit for a resource exists.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](_index_d_._plugin_.uri.md) | A resource identifier. |

**Returns:** boolean

`true` if the given resource will be touched by this edit.

___

### insert

▸ **insert**(`uri`: [Uri](_index_d_._plugin_.uri.md), `position`: [Position](_index_d_._plugin_.position.md), `newText`: string, `metadata?`: [WorkspaceEditEntryMetadata](../interfaces/_index_d_._plugin_.workspaceeditentrymetadata.md)): void

*Defined in [index.d.ts:3231](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3231)*

Insert the given text at the given position.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](_index_d_._plugin_.uri.md) | A resource identifier. |
`position` | [Position](_index_d_._plugin_.position.md) | A position. |
`newText` | string | A string. |
`metadata?` | [WorkspaceEditEntryMetadata](../interfaces/_index_d_._plugin_.workspaceeditentrymetadata.md) | Optional metadata for the entry.  |

**Returns:** void

___

### renameFile

▸ **renameFile**(`oldUri`: [Uri](_index_d_._plugin_.uri.md), `newUri`: [Uri](_index_d_._plugin_.uri.md), `options?`: { ignoreIfExists?: boolean ; overwrite?: boolean  }, `metadata?`: [WorkspaceEditEntryMetadata](../interfaces/_index_d_._plugin_.workspaceeditentrymetadata.md)): void

*Defined in [index.d.ts:3295](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3295)*

Rename a file or folder.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`oldUri` | [Uri](_index_d_._plugin_.uri.md) | The existing file. |
`newUri` | [Uri](_index_d_._plugin_.uri.md) | The new location. |
`options?` | { ignoreIfExists?: boolean ; overwrite?: boolean  } | Defines if existing files should be overwritten or be ignored. When overwrite and ignoreIfExists are both set overwrite wins. |
`metadata?` | [WorkspaceEditEntryMetadata](../interfaces/_index_d_._plugin_.workspaceeditentrymetadata.md) | Optional metadata for the entry.  |

**Returns:** void

___

### replace

▸ **replace**(`uri`: [Uri](_index_d_._plugin_.uri.md), `range`: [Range](_index_d_._plugin_.range.md), `newText`: string, `metadata?`: [WorkspaceEditEntryMetadata](../interfaces/_index_d_._plugin_.workspaceeditentrymetadata.md)): void

*Defined in [index.d.ts:3221](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3221)*

Replace the given range with given text for the given resource.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](_index_d_._plugin_.uri.md) | A resource identifier. |
`range` | [Range](_index_d_._plugin_.range.md) | A range. |
`newText` | string | A string. |
`metadata?` | [WorkspaceEditEntryMetadata](../interfaces/_index_d_._plugin_.workspaceeditentrymetadata.md) | Optional metadata for the entry.  |

**Returns:** void

___

### set

▸ **set**(`uri`: [Uri](_index_d_._plugin_.uri.md), `edits`: [TextEdit](_index_d_._plugin_.textedit.md)[]): void

*Defined in [index.d.ts:3256](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3256)*

Set (and replace) text edits for a resource.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](_index_d_._plugin_.uri.md) | A resource identifier. |
`edits` | [TextEdit](_index_d_._plugin_.textedit.md)[] | An array of text edits.  |

**Returns:** void
