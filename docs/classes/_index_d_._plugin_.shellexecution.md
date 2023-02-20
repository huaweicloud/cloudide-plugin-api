**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ShellExecution

# Class: ShellExecution

## Hierarchy

* **ShellExecution**

## Index

### Constructors

* [constructor](_index_d_._plugin_.shellexecution.md#constructor)

### Properties

* [args](_index_d_._plugin_.shellexecution.md#args)
* [command](_index_d_._plugin_.shellexecution.md#command)
* [commandLine](_index_d_._plugin_.shellexecution.md#commandline)
* [options](_index_d_._plugin_.shellexecution.md#options)

## Constructors

### constructor

\+ **new ShellExecution**(`commandLine`: string, `options?`: [ShellExecutionOptions](../interfaces/_index_d_._plugin_.shellexecutionoptions.md)): [ShellExecution](_index_d_._plugin_.shellexecution.md)

*Defined in [index.d.ts:6464](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6464)*

Creates a shell execution with a full command line.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`commandLine` | string | The command line to execute. |
`options?` | [ShellExecutionOptions](../interfaces/_index_d_._plugin_.shellexecutionoptions.md) | Optional options for the started the shell.  |

**Returns:** [ShellExecution](_index_d_._plugin_.shellexecution.md)

\+ **new ShellExecution**(`command`: string \| [ShellQuotedString](../interfaces/_index_d_._plugin_.shellquotedstring.md), `args`: (string \| [ShellQuotedString](../interfaces/_index_d_._plugin_.shellquotedstring.md))[], `options?`: [ShellExecutionOptions](../interfaces/_index_d_._plugin_.shellexecutionoptions.md)): [ShellExecution](_index_d_._plugin_.shellexecution.md)

*Defined in [index.d.ts:6471](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6471)*

Creates a shell execution with a command and arguments. For the real execution VS Code will
construct a command line from the command and the arguments. This is subject to interpretation
especially when it comes to quoting. If full control over the command line is needed please
use the constructor that creates a `ShellExecution` with the full command line.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`command` | string \| [ShellQuotedString](../interfaces/_index_d_._plugin_.shellquotedstring.md) | The command to execute. |
`args` | (string \| [ShellQuotedString](../interfaces/_index_d_._plugin_.shellquotedstring.md))[] | The command arguments. |
`options?` | [ShellExecutionOptions](../interfaces/_index_d_._plugin_.shellexecutionoptions.md) | Optional options for the started the shell.  |

**Returns:** [ShellExecution](_index_d_._plugin_.shellexecution.md)

## Properties

### args

•  **args**: (string \| [ShellQuotedString](../interfaces/_index_d_._plugin_.shellquotedstring.md))[]

*Defined in [index.d.ts:6498](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6498)*

The shell args. Is `undefined` if created with a full command line.

___

### command

•  **command**: string \| [ShellQuotedString](../interfaces/_index_d_._plugin_.shellquotedstring.md)

*Defined in [index.d.ts:6493](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6493)*

The shell command. Is `undefined` if created with a full command line.

___

### commandLine

•  **commandLine**: string \| undefined

*Defined in [index.d.ts:6488](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6488)*

The shell command line. Is `undefined` if created with a command and arguments.

___

### options

• `Optional` **options**: [ShellExecutionOptions](../interfaces/_index_d_._plugin_.shellexecutionoptions.md)

*Defined in [index.d.ts:6504](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6504)*

The shell options used when the command line is executed in a shell.
Defaults to undefined.
