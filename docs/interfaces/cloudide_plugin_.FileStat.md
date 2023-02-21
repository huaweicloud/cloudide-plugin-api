[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / FileStat

# Interface: FileStat

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).FileStat

The `FileStat`-type represents metadata about a file

## Table of contents

### Properties

- [ctime](cloudide_plugin_.FileStat.md#ctime)
- [mtime](cloudide_plugin_.FileStat.md#mtime)
- [size](cloudide_plugin_.FileStat.md#size)
- [type](cloudide_plugin_.FileStat.md#type)

## Properties

### ctime

• **ctime**: `number`

The creation timestamp in milliseconds elapsed since January 1, 1970 00:00:00 UTC.

#### Defined in

[index.d.ts:5632](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5632)

___

### mtime

• **mtime**: `number`

The modification timestamp in milliseconds elapsed since January 1, 1970 00:00:00 UTC.

*Note:* If the file changed, it is important to provide an updated `mtime` that advanced
from the previous value. Otherwise there may be optimizations in place that will not show
the updated file contents in an editor for example.

#### Defined in

[index.d.ts:5640](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5640)

___

### size

• **size**: `number`

The size in bytes.

*Note:* If the file changed, it is important to provide an updated `size`. Otherwise there
may be optimizations in place that will not show the updated file contents in an editor for
example.

#### Defined in

[index.d.ts:5648](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5648)

___

### type

• **type**: [`FileType`](../enums/cloudide_plugin_.FileType.md)

The type of the file, e.g. is a regular file, a directory, or symbolic link
to a file.

*Note:* This value might be a bitmask, e.g. `FileType.File | FileType.SymbolicLink`.

#### Defined in

[index.d.ts:5628](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5628)
