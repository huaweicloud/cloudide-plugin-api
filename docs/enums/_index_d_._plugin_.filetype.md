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

*Defined in [index.d.ts:6841](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6841)*

A directory.

___

### File

•  **File**:  = 1

*Defined in [index.d.ts:6837](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6837)*

A regular file.

___

### SymbolicLink

•  **SymbolicLink**:  = 64

*Defined in [index.d.ts:6845](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6845)*

A symbolic link to a file.

___

### Unknown

•  **Unknown**:  = 0

*Defined in [index.d.ts:6833](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6833)*

The file type is unknown.
