**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugAdapterExecutable

# Class: DebugAdapterExecutable

Represents a debug adapter executable and optional arguments and runtime options passed to it.

## Hierarchy

* **DebugAdapterExecutable**

## Index

### Constructors

* [constructor](_index_d_._plugin_.debugadapterexecutable.md#constructor)

### Properties

* [args](_index_d_._plugin_.debugadapterexecutable.md#args)
* [command](_index_d_._plugin_.debugadapterexecutable.md#command)
* [options](_index_d_._plugin_.debugadapterexecutable.md#options)

## Constructors

### constructor

\+ **new DebugAdapterExecutable**(`command`: string, `args?`: string[], `options?`: [DebugAdapterExecutableOptions](../interfaces/_index_d_._plugin_.debugadapterexecutableoptions.md)): [DebugAdapterExecutable](_index_d_._plugin_.debugadapterexecutable.md)

*Defined in [index.d.ts:11658](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11658)*

Creates a description for a debug adapter based on an executable program.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`command` | string | The command or executable path that implements the debug adapter. |
`args?` | string[] | Optional arguments to be passed to the command or executable. |
`options?` | [DebugAdapterExecutableOptions](../interfaces/_index_d_._plugin_.debugadapterexecutableoptions.md) | Optional options to be used when starting the command or executable.  |

**Returns:** [DebugAdapterExecutable](_index_d_._plugin_.debugadapterexecutable.md)

## Properties

### args

• `Readonly` **args**: string[]

*Defined in [index.d.ts:11679](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11679)*

The arguments passed to the debug adapter executable. Defaults to an empty array.

___

### command

• `Readonly` **command**: string

*Defined in [index.d.ts:11674](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11674)*

The command or path of the debug adapter executable.
A command must be either an absolute path of an executable or the name of an command to be looked up via the PATH environment variable.
The special value 'node' will be mapped to VS Code's built-in Node.js runtime.

___

### options

• `Optional` `Readonly` **options**: [DebugAdapterExecutableOptions](../interfaces/_index_d_._plugin_.debugadapterexecutableoptions.md)

*Defined in [index.d.ts:11685](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11685)*

Optional options to be used when the debug adapter is started.
Defaults to undefined.
