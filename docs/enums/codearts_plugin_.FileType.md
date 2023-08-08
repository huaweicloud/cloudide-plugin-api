[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileType

# Enumeration: FileType

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileType

Enumeration of file types. The types `File` and `Directory` can also be
a symbolic links, in that case use `FileType.File | FileType.SymbolicLink` and
`FileType.Directory | FileType.SymbolicLink`.

## Table of contents

### Enumeration Members

- [Directory](codearts_plugin_.FileType.md#directory)
- [File](codearts_plugin_.FileType.md#file)
- [SymbolicLink](codearts_plugin_.FileType.md#symboliclink)
- [Unknown](codearts_plugin_.FileType.md#unknown)

## Enumeration Members

### Directory

• **Directory** = ``2``

A directory.

#### Defined in

[index.d.ts:7882](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7882)

___

### File

• **File** = ``1``

A regular file.

#### Defined in

[index.d.ts:7878](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7878)

___

### SymbolicLink

• **SymbolicLink** = ``64``

A symbolic link to a file.

#### Defined in

[index.d.ts:7886](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7886)

___

### Unknown

• **Unknown** = ``0``

The file type is unknown.

#### Defined in

[index.d.ts:7874](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7874)
