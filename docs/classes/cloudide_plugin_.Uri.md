[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Uri

# Class: Uri

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Uri

A universal resource identifier representing either a file on disk
or another resource, like untitled resources.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.Uri.md#constructor)

### Properties

- [authority](cloudide_plugin_.Uri.md#authority)
- [fragment](cloudide_plugin_.Uri.md#fragment)
- [fsPath](cloudide_plugin_.Uri.md#fspath)
- [path](cloudide_plugin_.Uri.md#path)
- [query](cloudide_plugin_.Uri.md#query)
- [scheme](cloudide_plugin_.Uri.md#scheme)

### Methods

- [toJSON](cloudide_plugin_.Uri.md#tojson)
- [toString](cloudide_plugin_.Uri.md#tostring)
- [with](cloudide_plugin_.Uri.md#with)
- [file](cloudide_plugin_.Uri.md#file)
- [joinPath](cloudide_plugin_.Uri.md#joinpath)
- [parse](cloudide_plugin_.Uri.md#parse)

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

[index.d.ts:1383](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1383)

## Properties

### authority

• `Readonly` **authority**: `string`

Authority is the `www.msft.com` part of `http://www.msft.com/some/path?query#fragment`.
The part between the first double slashes and the next slash.

#### Defined in

[index.d.ts:1395](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1395)

___

### fragment

• `Readonly` **fragment**: `string`

Fragment is the `fragment` part of `http://www.msft.com/some/path?query#fragment`.

#### Defined in

[index.d.ts:1410](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1410)

___

### fsPath

• `Readonly` **fsPath**: `string`

The string representing the corresponding file system path of this Uri.

Will handle UNC paths and normalize windows drive letters to lower-case. Also
uses the platform specific path separator. Will *not* validate the path for
invalid characters and semantics. Will *not* look at the scheme of this Uri.

#### Defined in

[index.d.ts:1419](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1419)

___

### path

• `Readonly` **path**: `string`

Path is the `/some/path` part of `http://www.msft.com/some/path?query#fragment`.

#### Defined in

[index.d.ts:1400](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1400)

___

### query

• `Readonly` **query**: `string`

Query is the `query` part of `http://www.msft.com/some/path?query#fragment`.

#### Defined in

[index.d.ts:1405](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1405)

___

### scheme

• `Readonly` **scheme**: `string`

Scheme is the `http` part of `http://www.msft.com/some/path?query#fragment`.
The part before the first colon.

#### Defined in

[index.d.ts:1389](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1389)

## Methods

### toJSON

▸ **toJSON**(): `any`

Returns a JSON representation of this Uri.

#### Returns

`any`

An object.

#### Defined in

[index.d.ts:1453](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1453)

___

### toString

▸ **toString**(`skipEncoding?`): `string`

Returns a string representation of this Uri. The representation and normalization
of a URI depends on the scheme. The resulting string can be safely used with
[Uri.parse](#Uri.parse).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `skipEncoding?` | `boolean` | Do not percentage-encode the result, defaults to `false`. Note that the `#` and `?` characters occurring in the path will always be encoded. |

#### Returns

`string`

A string representation of this Uri.

#### Defined in

[index.d.ts:1446](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1446)

___

### with

▸ **with**(`change`): [`Uri`](cloudide_plugin_.Uri.md)

Derive a new Uri from this Uri.

```ts
let file = Uri.parse('before:some/file/path');
let other = file.with({ scheme: 'after' });
assert.ok(other.toString() === 'after:some/file/path');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `change` | `Object` | An object that describes a change to this Uri. To unset components use `null` or the empty string. |
| `change.authority?` | `string` | - |
| `change.fragment?` | `string` | - |
| `change.path?` | `string` | - |
| `change.query?` | `string` | - |
| `change.scheme?` | `string` | - |

#### Returns

[`Uri`](cloudide_plugin_.Uri.md)

A new Uri that reflects the given change. Will return `this` Uri if the change
 is not changing anything.

#### Defined in

[index.d.ts:1435](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1435)

___

### file

▸ `Static` **file**(`path`): [`Uri`](cloudide_plugin_.Uri.md)

Create an URI from a file system path. The [scheme](#Uri.scheme)
will be `file`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | A file system or UNC path. |

#### Returns

[`Uri`](cloudide_plugin_.Uri.md)

A new Uri instance.

#### Defined in

[index.d.ts:1348](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1348)

___

### joinPath

▸ `Static` **joinPath**(`uri`, `...pathSegments`): `URI`

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
| `uri` | `URI` | - |
| `...pathSegments` | `string`[] | One more more path fragments |

#### Returns

`URI`

A new uri which path is joined with the given fragments

#### Defined in

[index.d.ts:1369](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1369)

___

### parse

▸ `Static` **parse**(`value`): [`Uri`](cloudide_plugin_.Uri.md)

Create an URI from a string. Will throw if the given value is not
valid.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | The string value of an Uri. |

#### Returns

[`Uri`](cloudide_plugin_.Uri.md)

A new Uri instance.

#### Defined in

[index.d.ts:1378](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1378)
