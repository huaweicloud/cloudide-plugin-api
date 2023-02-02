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

[index.d.ts:7918](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7918)

## Properties

### code

• `Readonly` **code**: `string`

A code that identifies this error.

Possible values are names of errors, like [`FileNotFound`](codearts_plugin_.FileSystemError.md#filenotfound),
or `Unknown` for unspecified errors.

#### Defined in

[index.d.ts:7926](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7926)

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

[index.d.ts:7886](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7886)

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

[index.d.ts:7898](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7898)

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

[index.d.ts:7892](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7892)

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

[index.d.ts:7879](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7879)

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

[index.d.ts:7904](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7904)

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

[index.d.ts:7911](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7911)
