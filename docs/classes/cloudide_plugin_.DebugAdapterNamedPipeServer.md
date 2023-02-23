[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DebugAdapterNamedPipeServer

# Class: DebugAdapterNamedPipeServer

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DebugAdapterNamedPipeServer

Represents a debug adapter running as a Named Pipe (on Windows)/UNIX Domain Socket (on non-Windows) based server.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.DebugAdapterNamedPipeServer.md#constructor)

### Properties

- [path](cloudide_plugin_.DebugAdapterNamedPipeServer.md#path)

## Constructors

### constructor

• **new DebugAdapterNamedPipeServer**(`path`)

Create a description for a debug adapter running as a Named Pipe (on Windows)/UNIX Domain Socket (on non-Windows) based server.

#### Parameters

| Name | Type |
| :------ | :------ |
| `path` | `string` |

#### Defined in

[index.d.ts:9848](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9848)

## Properties

### path

• `Readonly` **path**: `string`

The path to the NamedPipe/UNIX Domain Socket.

#### Defined in

[index.d.ts:9843](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9843)
