[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DebugAdapterExecutable

# Class: DebugAdapterExecutable

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DebugAdapterExecutable

Represents a debug adapter executable and optional arguments and runtime options passed to it.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.DebugAdapterExecutable.md#constructor)

### Properties

- [args](cloudide_plugin_.DebugAdapterExecutable.md#args)
- [command](cloudide_plugin_.DebugAdapterExecutable.md#command)
- [options](cloudide_plugin_.DebugAdapterExecutable.md#options)

## Constructors

### constructor

• **new DebugAdapterExecutable**(`command`, `args?`, `options?`)

Creates a description for a debug adapter based on an executable program.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `command` | `string` | The command or executable path that implements the debug adapter. |
| `args?` | `string`[] | Optional arguments to be passed to the command or executable. |
| `options?` | [`DebugAdapterExecutableOptions`](../interfaces/cloudide_plugin_.DebugAdapterExecutableOptions.md) | Optional options to be used when starting the command or executable. |

#### Defined in

[index.d.ts:9776](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9776)

## Properties

### args

• `Readonly` **args**: `string`[]

The arguments passed to the debug adapter executable. Defaults to an empty array.

#### Defined in

[index.d.ts:9788](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9788)

___

### command

• `Readonly` **command**: `string`

The command or path of the debug adapter executable.
A command must be either an absolute path of an executable or the name of an command to be looked up via the PATH environment variable.
The special value 'node' will be mapped to VS Code's built-in Node.js runtime.

#### Defined in

[index.d.ts:9783](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9783)

___

### options

• `Optional` `Readonly` **options**: [`DebugAdapterExecutableOptions`](../interfaces/cloudide_plugin_.DebugAdapterExecutableOptions.md)

Optional options to be used when the debug adapter is started.
Defaults to undefined.

#### Defined in

[index.d.ts:9794](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9794)
