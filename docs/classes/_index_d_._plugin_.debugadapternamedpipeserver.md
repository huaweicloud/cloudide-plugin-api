**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugAdapterNamedPipeServer

# Class: DebugAdapterNamedPipeServer

Represents a debug adapter running as a Named Pipe (on Windows)/UNIX Domain Socket (on non-Windows) based server.

## Hierarchy

* **DebugAdapterNamedPipeServer**

## Index

### Constructors

* [constructor](_index_d_._plugin_.debugadapternamedpipeserver.md#constructor)

### Properties

* [path](_index_d_._plugin_.debugadapternamedpipeserver.md#path)

## Constructors

### constructor

\+ **new DebugAdapterNamedPipeServer**(`path`: string): [DebugAdapterNamedPipeServer](_index_d_._plugin_.debugadapternamedpipeserver.md)

*Defined in [index.d.ts:11734](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11734)*

Create a description for a debug adapter running as a socket based server.

#### Parameters:

Name | Type |
------ | ------ |
`path` | string |

**Returns:** [DebugAdapterNamedPipeServer](_index_d_._plugin_.debugadapternamedpipeserver.md)

## Properties

### path

• `Readonly` **path**: string

*Defined in [index.d.ts:11734](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11734)*

The path to the NamedPipe/UNIX Domain Socket.
