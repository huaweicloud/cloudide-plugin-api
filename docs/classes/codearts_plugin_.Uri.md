[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Uri

# Class: Uri

["@codearts/plugin"](../modules/_codearts_plugin_.md).Uri

A universal resource identifier representing either a file on disk
or another resource, like untitled resources.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.Uri.md#constructor)

### Properties

- [authority](codearts_plugin_.Uri.md#authority)
- [fragment](codearts_plugin_.Uri.md#fragment)
- [fsPath](codearts_plugin_.Uri.md#fspath)
- [path](codearts_plugin_.Uri.md#path)
- [query](codearts_plugin_.Uri.md#query)
- [scheme](codearts_plugin_.Uri.md#scheme)

### Methods

- [toJSON](codearts_plugin_.Uri.md#tojson)
- [toString](codearts_plugin_.Uri.md#tostring)
- [with](codearts_plugin_.Uri.md#with)
- [file](codearts_plugin_.Uri.md#file)
- [from](codearts_plugin_.Uri.md#from)
- [joinPath](codearts_plugin_.Uri.md#joinpath)
- [parse](codearts_plugin_.Uri.md#parse)

## Constructors

### constructor

• `Private` **new Uri**(`scheme`, `authority`, `path`, `query`, `fragment`)

Use the `file` and `parse` factory functions to create new `Uri` objects.

#### Parameters

| Name | Type |
| :------ | :------ |
| `scheme` | `string` |
| `authority` | `string` |
| `path` | `string` |
| `query` | `string` |
| `fragment` | `string` |

#### Defined in

[index.d.ts:1399](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1399)

## Properties

### authority

• `Readonly` **authority**: `string`

Authority is the `www.example.com` part of `http://www.example.com/some/path?query#fragment`.
The part between the first double slashes and the next slash.

#### Defined in

[index.d.ts:1411](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1411)

___

### fragment

• `Readonly` **fragment**: `string`

Fragment is the `fragment` part of `http://www.example.com/some/path?query#fragment`.

#### Defined in

[index.d.ts:1426](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1426)

___

### fsPath

• `Readonly` **fsPath**: `string`

The string representing the corresponding file system path of this Uri.

Will handle UNC paths and normalize windows drive letters to lower-case. Also
uses the platform specific path separator.

* Will *not* validate the path for invalid characters and semantics.
* Will *not* look at the scheme of this Uri.
* The resulting string shall *not* be used for display purposes but
for disk operations, like `readFile` et al.

The *difference* to the [`path`](codearts_plugin_.Uri.md#path)-property is the use of the platform specific
path separator and the handling of UNC paths. The sample below outlines the difference:
```ts
const u = URI.parse('file://server/c$/folder/file.txt')
u.authority === 'server'
u.path === '/shares/c$/file.txt'
u.fsPath === '\\server\c$\folder\file.txt'
```

#### Defined in

[index.d.ts:1448](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1448)

___

### path

• `Readonly` **path**: `string`

Path is the `/some/path` part of `http://www.example.com/some/path?query#fragment`.

#### Defined in

[index.d.ts:1416](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1416)

___

### query

• `Readonly` **query**: `string`

Query is the `query` part of `http://www.example.com/some/path?query#fragment`.

#### Defined in

[index.d.ts:1421](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1421)

___

### scheme

• `Readonly` **scheme**: `string`

Scheme is the `http` part of `http://www.example.com/some/path?query#fragment`.
The part before the first colon.

#### Defined in

[index.d.ts:1405](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1405)

## Methods

### toJSON

▸ **toJSON**(): `any`

Returns a JSON representation of this Uri.

#### Returns

`any`

An object.

#### Defined in

[index.d.ts:1490](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1490)

___

### toString

▸ **toString**(`skipEncoding?`): `string`

Returns a string representation of this Uri. The representation and normalization
of a URI depends on the scheme.

* The resulting string can be safely used with [parse](codearts_plugin_.Uri.md#parse).
* The resulting string shall *not* be used for display purposes.

*Note* that the implementation will encode _aggressive_ which often leads to unexpected,
but not incorrect, results. For instance, colons are encoded to `%3A` which might be unexpected
in file-uri. Also `&` and `=` will be encoded which might be unexpected for http-uris. For stability
reasons this cannot be changed anymore. If you suffer from too aggressive encoding you should use
the `skipEncoding`-argument: `uri.toString(true)`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `skipEncoding?` | `boolean` | Do not percentage-encode the result, defaults to `false`. Note that  the `#` and `?` characters occurring in the path will always be encoded. |

#### Returns

`string`

A string representation of this Uri.

#### Defined in

[index.d.ts:1483](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1483)

___

### with

▸ **with**(`change`): [`Uri`](codearts_plugin_.Uri.md)

Derive a new Uri from this Uri.

```ts
let file = Uri.parse('before:some/file/path');
let other = file.with({ scheme: 'after' });
assert.ok(other.toString() === 'after:some/file/path');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `change` | `Object` | An object that describes a change to this Uri. To unset components use `null` or  the empty string. |
| `change.authority?` | `string` | - |
| `change.fragment?` | `string` | - |
| `change.path?` | `string` | - |
| `change.query?` | `string` | - |
| `change.scheme?` | `string` | - |

#### Returns

[`Uri`](codearts_plugin_.Uri.md)

A new Uri that reflects the given change. Will return `this` Uri if the change
 is not changing anything.

#### Defined in

[index.d.ts:1464](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1464)

___

### file

▸ `Static` **file**(`path`): [`Uri`](codearts_plugin_.Uri.md)

Create an URI from a file system path. The [scheme](codearts_plugin_.Uri.md#scheme)
will be `file`.

The *difference* between [parse](codearts_plugin_.Uri.md#parse) and [file](codearts_plugin_.Uri.md#file) is that the latter treats the argument
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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | A file system or UNC path. |

#### Returns

[`Uri`](codearts_plugin_.Uri.md)

A new Uri instance.

#### Defined in

[index.d.ts:1363](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1363)

___

### from

▸ `Static` **from**(`components`): [`Uri`](codearts_plugin_.Uri.md)

Create an URI from its component parts

**`See`**

[toString](codearts_plugin_.Uri.md#tostring)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `components` | `Object` | The component parts of an Uri. |
| `components.authority?` | `string` | - |
| `components.fragment?` | `string` | - |
| `components.path?` | `string` | - |
| `components.query?` | `string` | - |
| `components.scheme` | `string` | - |

#### Returns

[`Uri`](codearts_plugin_.Uri.md)

A new Uri instance.

#### Defined in

[index.d.ts:1394](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1394)

___

### joinPath

▸ `Static` **joinPath**(`base`, ...`pathSegments`): [`Uri`](codearts_plugin_.Uri.md)

Create a new uri which path is the result of joining
the path of the base uri with the provided path segments.

- Note 1: `joinPath` only affects the path component
and all other components (scheme, authority, query, and fragment) are
left as they are.
- Note 2: The base uri must have a path; an error is thrown otherwise.

The path segments are normalized in the following ways:
- sequences of path separators (`/` or `\`) are replaced with a single separator
- for `file`-uris on windows, the backslash-character (``) is considered a path-separator
- the `..`-segment denotes the parent segment, the `.` denotes the current segment
- paths have a root which always remains, for instance on windows drive-letters are roots
so that is true: `joinPath(Uri.file('file:///c:/root'), '../../other').fsPath === 'c:/other'`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `base` | [`Uri`](codearts_plugin_.Uri.md) | An uri. Must have a path. |
| `...pathSegments` | `string`[] | One more more path fragments |

#### Returns

[`Uri`](codearts_plugin_.Uri.md)

A new uri which path is joined with the given fragments

#### Defined in

[index.d.ts:1385](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1385)

___

### parse

▸ `Static` **parse**(`value`, `strict?`): [`Uri`](codearts_plugin_.Uri.md)

Create an URI from a string, e.g. `http://www.example.com/some/path`,
`file:///usr/home`, or `scheme:with/path`.

*Note* that for a while uris without a `scheme` were accepted. That is not correct
as all uris should have a scheme. To avoid breakage of existing code the optional
`strict`-argument has been added. We *strongly* advise to use it, e.g. `Uri.parse('my:uri', true)`

**`See`**

[toString](codearts_plugin_.Uri.md#tostring)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | The string value of an Uri. |
| `strict?` | `boolean` | Throw an error when `value` is empty or when no `scheme` can be parsed. |

#### Returns

[`Uri`](codearts_plugin_.Uri.md)

A new Uri instance.

#### Defined in

[index.d.ts:1338](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1338)
