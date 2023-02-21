[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / FileSystemError

# Class: FileSystemError

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).FileSystemError

A type that filesystem providers should use to signal errors.

This class has factory methods for common error-cases, like `FileNotFound` when
a file or folder doesn't exist, use them like so: `throw vscode.FileSystemError.FileNotFound(someUri);`

## Hierarchy

- `Error`

  ↳ **`FileSystemError`**

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.FileSystemError.md#constructor)

### Properties

- [code](cloudide_plugin_.FileSystemError.md#code)

### Methods

- [FileExists](cloudide_plugin_.FileSystemError.md#fileexists)
- [FileIsADirectory](cloudide_plugin_.FileSystemError.md#fileisadirectory)
- [FileNotADirectory](cloudide_plugin_.FileSystemError.md#filenotadirectory)
- [FileNotFound](cloudide_plugin_.FileSystemError.md#filenotfound)
- [NoPermissions](cloudide_plugin_.FileSystemError.md#nopermissions)
- [Unavailable](cloudide_plugin_.FileSystemError.md#unavailable)

## Constructors

### constructor

• **new FileSystemError**(`messageOrUri?`)

Creates a new filesystem error.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](cloudide_plugin_.Uri.md) | Message or uri. |

#### Overrides

Error.constructor

#### Defined in

[index.d.ts:5702](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5702)

## Properties

### code

• `Readonly` **code**: `string`

A code that identifies this error.

Possible values are names of errors, like [`FileNotFound`](#FileSystemError.FileNotFound),
or `Unknown` for unspecified errors.

#### Defined in

[index.d.ts:5710](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5710)

## Methods

### FileExists

▸ `Static` **FileExists**(`messageOrUri?`): [`FileSystemError`](cloudide_plugin_.FileSystemError.md)

Create an error to signal that a file or folder already exists, e.g. when
creating but not overwriting a file.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](cloudide_plugin_.Uri.md) | Message or uri. |

#### Returns

[`FileSystemError`](cloudide_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:5670](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5670)

___

### FileIsADirectory

▸ `Static` **FileIsADirectory**(`messageOrUri?`): [`FileSystemError`](cloudide_plugin_.FileSystemError.md)

Create an error to signal that a file is a folder.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](cloudide_plugin_.Uri.md) | Message or uri. |

#### Returns

[`FileSystemError`](cloudide_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:5682](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5682)

___

### FileNotADirectory

▸ `Static` **FileNotADirectory**(`messageOrUri?`): [`FileSystemError`](cloudide_plugin_.FileSystemError.md)

Create an error to signal that a file is not a folder.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](cloudide_plugin_.Uri.md) | Message or uri. |

#### Returns

[`FileSystemError`](cloudide_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:5676](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5676)

___

### FileNotFound

▸ `Static` **FileNotFound**(`messageOrUri?`): [`FileSystemError`](cloudide_plugin_.FileSystemError.md)

Create an error to signal that a file or folder wasn't found.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](cloudide_plugin_.Uri.md) | Message or uri. |

#### Returns

[`FileSystemError`](cloudide_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:5663](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5663)

___

### NoPermissions

▸ `Static` **NoPermissions**(`messageOrUri?`): [`FileSystemError`](cloudide_plugin_.FileSystemError.md)

Create an error to signal that an operation lacks required permissions.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](cloudide_plugin_.Uri.md) | Message or uri. |

#### Returns

[`FileSystemError`](cloudide_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:5688](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5688)

___

### Unavailable

▸ `Static` **Unavailable**(`messageOrUri?`): [`FileSystemError`](cloudide_plugin_.FileSystemError.md)

Create an error to signal that the file system is unavailable or too busy to
complete a request.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](cloudide_plugin_.Uri.md) | Message or uri. |

#### Returns

[`FileSystemError`](cloudide_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:5695](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5695)
