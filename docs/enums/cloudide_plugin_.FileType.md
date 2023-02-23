[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / FileType

# Enumeration: FileType

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).FileType

Enumeration of file types. The types `File` and `Directory` can also be
a symbolic link, in that case use `FileType.File | FileType.SymbolicLink` and
`FileType.Directory | FileType.SymbolicLink`.

## Table of contents

### Enumeration Members

- [Directory](cloudide_plugin_.FileType.md#directory)
- [File](cloudide_plugin_.FileType.md#file)
- [SymbolicLink](cloudide_plugin_.FileType.md#symboliclink)
- [Unknown](cloudide_plugin_.FileType.md#unknown)

## Enumeration Members

### Directory

• **Directory** = ``2``

A directory.

#### Defined in

[index.d.ts:5611](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5611)

___

### File

• **File** = ``1``

A regular file.

#### Defined in

[index.d.ts:5607](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5607)

___

### SymbolicLink

• **SymbolicLink** = ``64``

A symbolic link to a file.

#### Defined in

[index.d.ts:5615](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5615)

___

### Unknown

• **Unknown** = ``0``

The file type is unknown.

#### Defined in

[index.d.ts:5603](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5603)
