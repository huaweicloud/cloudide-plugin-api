[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileSystemError

# Class: FileSystemError

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileSystemError

A type that filesystem providers should use to signal errors.

This class has factory methods for common error-cases, like `FileNotFound` when
a file or folder doesn't exist, use them like so: `throw vscode.FileSystemError.FileNotFound(someUri);`

## Hierarchy

- `Error`

  ↳ **`FileSystemError`**

## Table of contents

### Constructors

- [constructor](codearts_plugin_.FileSystemError.md#constructor)

### Properties

- [code](codearts_plugin_.FileSystemError.md#code)

### Methods

- [FileExists](codearts_plugin_.FileSystemError.md#fileexists)
- [FileIsADirectory](codearts_plugin_.FileSystemError.md#fileisadirectory)
- [FileNotADirectory](codearts_plugin_.FileSystemError.md#filenotadirectory)
- [FileNotFound](codearts_plugin_.FileSystemError.md#filenotfound)
- [NoPermissions](codearts_plugin_.FileSystemError.md#nopermissions)
- [Unavailable](codearts_plugin_.FileSystemError.md#unavailable)

## Constructors

### constructor

• **new FileSystemError**(`messageOrUri?`)

Creates a new filesystem error.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](codearts_plugin_.Uri.md) | Message or uri. |

#### Overrides

Error.constructor

#### Defined in

[index.d.ts:7991](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7991)

## Properties

### code

• `Readonly` **code**: `string`

A code that identifies this error.

Possible values are names of errors, like [`FileNotFound`](codearts_plugin_.FileSystemError.md#filenotfound),
or `Unknown` for unspecified errors.

#### Defined in

[index.d.ts:7999](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7999)

## Methods

### FileExists

▸ `Static` **FileExists**(`messageOrUri?`): [`FileSystemError`](codearts_plugin_.FileSystemError.md)

Create an error to signal that a file or folder already exists, e.g. when
creating but not overwriting a file.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](codearts_plugin_.Uri.md) | Message or uri. |

#### Returns

[`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:7959](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7959)

___

### FileIsADirectory

▸ `Static` **FileIsADirectory**(`messageOrUri?`): [`FileSystemError`](codearts_plugin_.FileSystemError.md)

Create an error to signal that a file is a folder.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](codearts_plugin_.Uri.md) | Message or uri. |

#### Returns

[`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:7971](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7971)

___

### FileNotADirectory

▸ `Static` **FileNotADirectory**(`messageOrUri?`): [`FileSystemError`](codearts_plugin_.FileSystemError.md)

Create an error to signal that a file is not a folder.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](codearts_plugin_.Uri.md) | Message or uri. |

#### Returns

[`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:7965](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7965)

___

### FileNotFound

▸ `Static` **FileNotFound**(`messageOrUri?`): [`FileSystemError`](codearts_plugin_.FileSystemError.md)

Create an error to signal that a file or folder wasn't found.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](codearts_plugin_.Uri.md) | Message or uri. |

#### Returns

[`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:7952](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7952)

___

### NoPermissions

▸ `Static` **NoPermissions**(`messageOrUri?`): [`FileSystemError`](codearts_plugin_.FileSystemError.md)

Create an error to signal that an operation lacks required permissions.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](codearts_plugin_.Uri.md) | Message or uri. |

#### Returns

[`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:7977](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7977)

___

### Unavailable

▸ `Static` **Unavailable**(`messageOrUri?`): [`FileSystemError`](codearts_plugin_.FileSystemError.md)

Create an error to signal that the file system is unavailable or too busy to
complete a request.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](codearts_plugin_.Uri.md) | Message or uri. |

#### Returns

[`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:7984](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7984)
