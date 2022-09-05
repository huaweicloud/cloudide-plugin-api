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

[index.d.ts:7784](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7784)

___

### File

• **File** = ``1``

A regular file.

#### Defined in

[index.d.ts:7780](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7780)

___

### SymbolicLink

• **SymbolicLink** = ``64``

A symbolic link to a file.

#### Defined in

[index.d.ts:7788](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7788)

___

### Unknown

• **Unknown** = ``0``

The file type is unknown.

#### Defined in

[index.d.ts:7776](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7776)
