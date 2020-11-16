**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FileType

# Enumeration: FileType

Enumeration of file types. The types `File` and `Directory` can also be
a symbolic links, in that case use `FileType.File | FileType.SymbolicLink` and
`FileType.Directory | FileType.SymbolicLink`.

## Index

### Enumeration members

* [Directory](_index_d_._plugin_.filetype.md#directory)
* [File](_index_d_._plugin_.filetype.md#file)
* [SymbolicLink](_index_d_._plugin_.filetype.md#symboliclink)
* [Unknown](_index_d_._plugin_.filetype.md#unknown)

## Enumeration members

### Directory

•  **Directory**:  = 2

*Defined in [index.d.ts:6232](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6232)*

A directory.

___

### File

•  **File**:  = 1

*Defined in [index.d.ts:6228](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6228)*

A regular file.

___

### SymbolicLink

•  **SymbolicLink**:  = 64

*Defined in [index.d.ts:6236](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6236)*

A symbolic link to a file.

___

### Unknown

•  **Unknown**:  = 0

*Defined in [index.d.ts:6224](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6224)*

The file type is unknown.
