[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugAdapterExecutable

# Class: DebugAdapterExecutable

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugAdapterExecutable

Represents a debug adapter executable and optional arguments and runtime options passed to it.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.DebugAdapterExecutable.md#constructor)

### Properties

- [args](codearts_plugin_.DebugAdapterExecutable.md#args)
- [command](codearts_plugin_.DebugAdapterExecutable.md#command)
- [options](codearts_plugin_.DebugAdapterExecutable.md#options)

## Constructors

### constructor

• **new DebugAdapterExecutable**(`command`, `args?`, `options?`)

Creates a description for a debug adapter based on an executable program.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `command` | `string` | The command or executable path that implements the debug adapter. |
| `args?` | `string`[] | Optional arguments to be passed to the command or executable. |
| `options?` | [`DebugAdapterExecutableOptions`](../interfaces/codearts_plugin_.DebugAdapterExecutableOptions.md) | Optional options to be used when starting the command or executable. |

#### Defined in

[index.d.ts:15155](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L15155)

## Properties

### args

• `Readonly` **args**: `string`[]

The arguments passed to the debug adapter executable. Defaults to an empty array.

#### Defined in

[index.d.ts:15167](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L15167)

___

### command

• `Readonly` **command**: `string`

The command or path of the debug adapter executable.
A command must be either an absolute path of an executable or the name of an command to be looked up via the PATH environment variable.
The special value 'node' will be mapped to the editor's built-in Node.js runtime.

#### Defined in

[index.d.ts:15162](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L15162)

___

### options

• `Optional` `Readonly` **options**: [`DebugAdapterExecutableOptions`](../interfaces/codearts_plugin_.DebugAdapterExecutableOptions.md)

Optional options to be used when the debug adapter is started.
Defaults to undefined.

#### Defined in

[index.d.ts:15173](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L15173)
