**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FileStat

# Interface: FileStat

The `FileStat`-type represents metadata about a file

## Hierarchy

* **FileStat**

## Index

### Properties

* [ctime](_index_d_._plugin_.filestat.md#ctime)
* [mtime](_index_d_._plugin_.filestat.md#mtime)
* [size](_index_d_._plugin_.filestat.md#size)
* [type](_index_d_._plugin_.filestat.md#type)

## Properties

### ctime

•  **ctime**: number

*Defined in [index.d.ts:6865](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6865)*

The creation timestamp in milliseconds elapsed since January 1, 1970 00:00:00 UTC.

___

### mtime

•  **mtime**: number

*Defined in [index.d.ts:6873](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6873)*

The modification timestamp in milliseconds elapsed since January 1, 1970 00:00:00 UTC.

*Note:* If the file changed, it is important to provide an updated `mtime` that advanced
from the previous value. Otherwise there may be optimizations in place that will not show
the updated file contents in an editor for example.

___

### size

•  **size**: number

*Defined in [index.d.ts:6881](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6881)*

The size in bytes.

*Note:* If the file changed, it is important to provide an updated `size`. Otherwise there
may be optimizations in place that will not show the updated file contents in an editor for
example.

___

### type

•  **type**: [FileType](../enums/_index_d_._plugin_.filetype.md)

*Defined in [index.d.ts:6861](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6861)*

The type of the file, e.g. is a regular file, a directory, or symbolic link
to a file.

*Note:* This value might be a bitmask, e.g. `FileType.File | FileType.SymbolicLink`.
