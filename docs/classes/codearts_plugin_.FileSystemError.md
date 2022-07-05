[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileSystemError

# Class: FileSystemError

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileSystemError

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](codearts_plugin_.Uri.md) |  |

#### Overrides

Error.constructor

#### Defined in

[index.d.ts:7893](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L7893)

## Properties

### code

• `Readonly` **code**: `string`

#### Defined in

[index.d.ts:7901](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L7901)

## Methods

### FileExists

▸ `Static` **FileExists**(`messageOrUri?`): [`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](codearts_plugin_.Uri.md) |  |

#### Returns

[`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:7861](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L7861)

___

### FileIsADirectory

▸ `Static` **FileIsADirectory**(`messageOrUri?`): [`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](codearts_plugin_.Uri.md) |  |

#### Returns

[`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:7873](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L7873)

___

### FileNotADirectory

▸ `Static` **FileNotADirectory**(`messageOrUri?`): [`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](codearts_plugin_.Uri.md) |  |

#### Returns

[`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:7867](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L7867)

___

### FileNotFound

▸ `Static` **FileNotFound**(`messageOrUri?`): [`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](codearts_plugin_.Uri.md) |  |

#### Returns

[`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:7854](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L7854)

___

### NoPermissions

▸ `Static` **NoPermissions**(`messageOrUri?`): [`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](codearts_plugin_.Uri.md) |  |

#### Returns

[`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:7879](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L7879)

___

### Unavailable

▸ `Static` **Unavailable**(`messageOrUri?`): [`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `messageOrUri?` | `string` \| [`Uri`](codearts_plugin_.Uri.md) |  |

#### Returns

[`FileSystemError`](codearts_plugin_.FileSystemError.md)

#### Defined in

[index.d.ts:7886](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L7886)
