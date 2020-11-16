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

*Defined in [index.d.ts:10218](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10218)*

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

*Defined in [index.d.ts:10239](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10239)*

The arguments passed to the debug adapter executable. Defaults to an empty array.

___

### command

• `Readonly` **command**: string

*Defined in [index.d.ts:10234](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10234)*

The command or path of the debug adapter executable.
A command must be either an absolute path of an executable or the name of an command to be looked up via the PATH environment variable.
The special value 'node' will be mapped to VS Code's built-in Node.js runtime.

___

### options

• `Optional` `Readonly` **options**: [DebugAdapterExecutableOptions](../interfaces/_index_d_._plugin_.debugadapterexecutableoptions.md)

*Defined in [index.d.ts:10245](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10245)*

Optional options to be used when the debug adapter is started.
Defaults to undefined.
