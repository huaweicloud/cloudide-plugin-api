**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FileSystemError

# Class: FileSystemError

A type that filesystem providers should use to signal errors.

This class has factory methods for common error-cases, like `FileNotFound` when
a file or folder doesn't exist, use them like so: `throw vscode.FileSystemError.FileNotFound(someUri);`

## Hierarchy

* [Error](_index_d_._plugin_.cancellationerror.md#error)

  ↳ **FileSystemError**

## Index

### Constructors

* [constructor](_index_d_._plugin_.filesystemerror.md#constructor)

### Properties

* [code](_index_d_._plugin_.filesystemerror.md#code)
* [message](_index_d_._plugin_.filesystemerror.md#message)
* [name](_index_d_._plugin_.filesystemerror.md#name)
* [stack](_index_d_._plugin_.filesystemerror.md#stack)
* [Error](_index_d_._plugin_.filesystemerror.md#error)

### Methods

* [FileExists](_index_d_._plugin_.filesystemerror.md#fileexists)
* [FileIsADirectory](_index_d_._plugin_.filesystemerror.md#fileisadirectory)
* [FileNotADirectory](_index_d_._plugin_.filesystemerror.md#filenotadirectory)
* [FileNotFound](_index_d_._plugin_.filesystemerror.md#filenotfound)
* [NoPermissions](_index_d_._plugin_.filesystemerror.md#nopermissions)
* [Unavailable](_index_d_._plugin_.filesystemerror.md#unavailable)

## Constructors

### constructor

\+ **new FileSystemError**(`messageOrUri?`: string \| [Uri](_index_d_._plugin_.uri.md)): [FileSystemError](_index_d_._plugin_.filesystemerror.md)

*Defined in [index.d.ts:6928](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6928)*

Creates a new filesystem error.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`messageOrUri?` | string \| [Uri](_index_d_._plugin_.uri.md) | Message or uri.  |

**Returns:** [FileSystemError](_index_d_._plugin_.filesystemerror.md)

## Properties

### code

• `Readonly` **code**: string

*Defined in [index.d.ts:6943](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6943)*

A code that identifies this error.

Possible values are names of errors, like [`FileNotFound`](#FileSystemError.FileNotFound),
or `Unknown` for unspecified errors.

___

### message

•  **message**: string

*Inherited from [CancellationError](_index_d_._plugin_.cancellationerror.md).[message](_index_d_._plugin_.cancellationerror.md#message)*

*Defined in node_modules/typescript/lib/lib.es5.d.ts:974*

___

### name

•  **name**: string

*Inherited from [CancellationError](_index_d_._plugin_.cancellationerror.md).[name](_index_d_._plugin_.cancellationerror.md#name)*

*Defined in node_modules/typescript/lib/lib.es5.d.ts:973*

___

### stack

• `Optional` **stack**: string

*Inherited from [CancellationError](_index_d_._plugin_.cancellationerror.md).[stack](_index_d_._plugin_.cancellationerror.md#stack)*

*Defined in node_modules/typescript/lib/lib.es5.d.ts:975*

___

### Error

▪ `Static` **Error**: ErrorConstructor

*Defined in node_modules/typescript/lib/lib.es5.d.ts:984*

## Methods

### FileExists

▸ `Static`**FileExists**(`messageOrUri?`: string \| [Uri](_index_d_._plugin_.uri.md)): [FileSystemError](_index_d_._plugin_.filesystemerror.md)

*Defined in [index.d.ts:6903](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6903)*

Create an error to signal that a file or folder already exists, e.g. when
creating but not overwriting a file.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`messageOrUri?` | string \| [Uri](_index_d_._plugin_.uri.md) | Message or uri.  |

**Returns:** [FileSystemError](_index_d_._plugin_.filesystemerror.md)

___

### FileIsADirectory

▸ `Static`**FileIsADirectory**(`messageOrUri?`: string \| [Uri](_index_d_._plugin_.uri.md)): [FileSystemError](_index_d_._plugin_.filesystemerror.md)

*Defined in [index.d.ts:6915](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6915)*

Create an error to signal that a file is a folder.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`messageOrUri?` | string \| [Uri](_index_d_._plugin_.uri.md) | Message or uri.  |

**Returns:** [FileSystemError](_index_d_._plugin_.filesystemerror.md)

___

### FileNotADirectory

▸ `Static`**FileNotADirectory**(`messageOrUri?`: string \| [Uri](_index_d_._plugin_.uri.md)): [FileSystemError](_index_d_._plugin_.filesystemerror.md)

*Defined in [index.d.ts:6909](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6909)*

Create an error to signal that a file is not a folder.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`messageOrUri?` | string \| [Uri](_index_d_._plugin_.uri.md) | Message or uri.  |

**Returns:** [FileSystemError](_index_d_._plugin_.filesystemerror.md)

___

### FileNotFound

▸ `Static`**FileNotFound**(`messageOrUri?`: string \| [Uri](_index_d_._plugin_.uri.md)): [FileSystemError](_index_d_._plugin_.filesystemerror.md)

*Defined in [index.d.ts:6896](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6896)*

Create an error to signal that a file or folder wasn't found.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`messageOrUri?` | string \| [Uri](_index_d_._plugin_.uri.md) | Message or uri.  |

**Returns:** [FileSystemError](_index_d_._plugin_.filesystemerror.md)

___

### NoPermissions

▸ `Static`**NoPermissions**(`messageOrUri?`: string \| [Uri](_index_d_._plugin_.uri.md)): [FileSystemError](_index_d_._plugin_.filesystemerror.md)

*Defined in [index.d.ts:6921](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6921)*

Create an error to signal that an operation lacks required permissions.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`messageOrUri?` | string \| [Uri](_index_d_._plugin_.uri.md) | Message or uri.  |

**Returns:** [FileSystemError](_index_d_._plugin_.filesystemerror.md)

___

### Unavailable

▸ `Static`**Unavailable**(`messageOrUri?`: string \| [Uri](_index_d_._plugin_.uri.md)): [FileSystemError](_index_d_._plugin_.filesystemerror.md)

*Defined in [index.d.ts:6928](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6928)*

Create an error to signal that the file system is unavailable or too busy to
complete a request.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`messageOrUri?` | string \| [Uri](_index_d_._plugin_.uri.md) | Message or uri.  |

**Returns:** [FileSystemError](_index_d_._plugin_.filesystemerror.md)
