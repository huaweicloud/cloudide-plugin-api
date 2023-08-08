[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugAdapterNamedPipeServer

# Class: DebugAdapterNamedPipeServer

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugAdapterNamedPipeServer

Represents a debug adapter running as a Named Pipe (on Windows)/UNIX Domain Socket (on non-Windows) based server.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.DebugAdapterNamedPipeServer.md#constructor)

### Properties

- [path](codearts_plugin_.DebugAdapterNamedPipeServer.md#path)

## Constructors

### constructor

• **new DebugAdapterNamedPipeServer**(`path`)

Create a description for a debug adapter running as a Named Pipe (on Windows)/UNIX Domain Socket (on non-Windows) based server.

#### Parameters

| Name | Type |
| :------ | :------ |
| `path` | `string` |

#### Defined in

[index.d.ts:15227](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L15227)

## Properties

### path

• `Readonly` **path**: `string`

The path to the NamedPipe/UNIX Domain Socket.

#### Defined in

[index.d.ts:15222](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L15222)
