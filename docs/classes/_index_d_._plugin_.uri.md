**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Uri

# Class: Uri

A universal resource identifier representing either a file on disk
or another resource, like untitled resources.

## Hierarchy

* **Uri**

## Index

### Constructors

* [constructor](_index_d_._plugin_.uri.md#constructor)

### Properties

* [authority](_index_d_._plugin_.uri.md#authority)
* [fragment](_index_d_._plugin_.uri.md#fragment)
* [fsPath](_index_d_._plugin_.uri.md#fspath)
* [path](_index_d_._plugin_.uri.md#path)
* [query](_index_d_._plugin_.uri.md#query)
* [scheme](_index_d_._plugin_.uri.md#scheme)

### Methods

* [toJSON](_index_d_._plugin_.uri.md#tojson)
* [toString](_index_d_._plugin_.uri.md#tostring)
* [with](_index_d_._plugin_.uri.md#with)
* [file](_index_d_._plugin_.uri.md#file)
* [joinPath](_index_d_._plugin_.uri.md#joinpath)
* [parse](_index_d_._plugin_.uri.md#parse)

## Constructors

### constructor

\+ `Private`**new Uri**(`scheme`: string, `authority`: string, `path`: string, `query`: string, `fragment`: string): [Uri](_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:1433](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1433)*

Use the `file` and `parse` factory functions to create new `Uri` objects.

#### Parameters:

Name | Type |
------ | ------ |
`scheme` | string |
`authority` | string |
`path` | string |
`query` | string |
`fragment` | string |

**Returns:** [Uri](_index_d_._plugin_.uri.md)

## Properties

### authority

• `Readonly` **authority**: string

*Defined in [index.d.ts:1450](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1450)*

Authority is the `www.msft.com` part of `http://www.msft.com/some/path?query#fragment`.
The part between the first double slashes and the next slash.

___

### fragment

• `Readonly` **fragment**: string

*Defined in [index.d.ts:1465](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1465)*

Fragment is the `fragment` part of `http://www.msft.com/some/path?query#fragment`.

___

### fsPath

• `Readonly` **fsPath**: string

*Defined in [index.d.ts:1487](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1487)*

The string representing the corresponding file system path of this Uri.

Will handle UNC paths and normalize windows drive letters to lower-case. Also
uses the platform specific path separator.

* Will *not* validate the path for invalid characters and semantics.
* Will *not* look at the scheme of this Uri.
* The resulting string shall *not* be used for display purposes but
for disk operations, like `readFile` et al.

The *difference* to the [`path`](#Uri.path)-property is the use of the platform specific
path separator and the handling of UNC paths. The sample below outlines the difference:
```ts
const u = URI.parse('file://server/c$/folder/file.txt')
u.authority === 'server'
u.path === '/shares/c$/file.txt'
u.fsPath === '\\server\c$\folder\file.txt'
```

___

### path

• `Readonly` **path**: string

*Defined in [index.d.ts:1455](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1455)*

Path is the `/some/path` part of `http://www.msft.com/some/path?query#fragment`.

___

### query

• `Readonly` **query**: string

*Defined in [index.d.ts:1460](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1460)*

Query is the `query` part of `http://www.msft.com/some/path?query#fragment`.

___

### scheme

• `Readonly` **scheme**: string

*Defined in [index.d.ts:1444](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1444)*

Scheme is the `http` part of `http://www.msft.com/some/path?query#fragment`.
The part before the first colon.

## Methods

### toJSON

▸ **toJSON**(): any

*Defined in [index.d.ts:1529](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1529)*

Returns a JSON representation of this Uri.

**Returns:** any

An object.

___

### toString

▸ **toString**(`skipEncoding?`: boolean): string

*Defined in [index.d.ts:1522](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1522)*

Returns a string representation of this Uri. The representation and normalization
of a URI depends on the scheme.

* The resulting string can be safely used with [Uri.parse](#Uri.parse).
* The resulting string shall *not* be used for display purposes.

*Note* that the implementation will encode _aggressive_ which often leads to unexpected,
but not incorrect, results. For instance, colons are encoded to `%3A` which might be unexpected
in file-uri. Also `&` and `=` will be encoded which might be unexpected for http-uris. For stability
reasons this cannot be changed anymore. If you suffer from too aggressive encoding you should use
the `skipEncoding`-argument: `uri.toString(true)`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`skipEncoding?` | boolean | Do not percentage-encode the result, defaults to `false`. Note that  the `#` and `?` characters occurring in the path will always be encoded. |

**Returns:** string

A string representation of this Uri.

___

### with

▸ **with**(`change`: { authority?: string ; fragment?: string ; path?: string ; query?: string ; scheme?: string  }): [Uri](_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:1503](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1503)*

Derive a new Uri from this Uri.

```ts
let file = Uri.parse('before:some/file/path');
let other = file.with({ scheme: 'after' });
assert.ok(other.toString() === 'after:some/file/path');
```

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`change` | { authority?: string ; fragment?: string ; path?: string ; query?: string ; scheme?: string  } | An object that describes a change to this Uri. To unset components use `null` or  the empty string. |

**Returns:** [Uri](_index_d_._plugin_.uri.md)

A new Uri that reflects the given change. Will return `this` Uri if the change
 is not changing anything.

___

### file

▸ `Static`**file**(`path`: string): [Uri](_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:1411](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1411)*

Create an URI from a file system path. The [scheme](#Uri.scheme)
will be `file`.

The *difference* between `Uri#parse` and `Uri#file` is that the latter treats the argument
as path, not as stringified-uri. E.g. `Uri.file(path)` is *not* the same as
`Uri.parse('file://' + path)` because the path might contain characters that are
interpreted (# and ?). See the following sample:
```ts
const good = URI.file('/coding/c#/project1');
good.scheme === 'file';
good.path === '/coding/c#/project1';
good.fragment === '';

const bad = URI.parse('file://' + '/coding/c#/project1');
bad.scheme === 'file';
bad.path === '/coding/c'; // path is now broken
bad.fragment === '/project1';
```

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`path` | string | A file system or UNC path. |

**Returns:** [Uri](_index_d_._plugin_.uri.md)

A new Uri instance.

___

### joinPath

▸ `Static`**joinPath**(`base`: [Uri](_index_d_._plugin_.uri.md), ...`pathSegments`: string[]): [Uri](_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:1433](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1433)*

Create a new uri which path is the result of joining
the path of the base uri with the provided path segments.

- Note 1: `joinPath` only affects the path component
and all other components (scheme, authority, query, and fragment) are
left as they are.
- Note 2: The base uri must have a path; an error is thrown otherwise.

The path segments are normalized in the following ways:
- sequences of path separators (`/` or `\`) are replaced with a single separator
- for `file`-uris on windows, the backslash-character (`\`) is considered a path-separator
- the `..`-segment denotes the parent segment, the `.` denotes the current segment
- paths have a root which always remains, for instance on windows drive-letters are roots
so that is true: `joinPath(Uri.file('file:///c:/root'), '../../other').fsPath === 'c:/other'`

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`base` | [Uri](_index_d_._plugin_.uri.md) | An uri. Must have a path. |
`...pathSegments` | string[] | One more more path fragments |

**Returns:** [Uri](_index_d_._plugin_.uri.md)

A new uri which path is joined with the given fragments

___

### parse

▸ `Static`**parse**(`value`: string, `strict?`: boolean): [Uri](_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:1386](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1386)*

Create an URI from a string, e.g. `http://www.msft.com/some/path`,
`file:///usr/home`, or `scheme:with/path`.

*Note* that for a while uris without a `scheme` were accepted. That is not correct
as all uris should have a scheme. To avoid breakage of existing code the optional
`strict`-argument has been added. We *strongly* advise to use it, e.g. `Uri.parse('my:uri', true)`

**`see`** [Uri.toString](#Uri.toString)

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`value` | string | The string value of an Uri. |
`strict?` | boolean | Throw an error when `value` is empty or when no `scheme` can be parsed. |

**Returns:** [Uri](_index_d_._plugin_.uri.md)

A new Uri instance.
