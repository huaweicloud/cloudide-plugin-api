[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ShellExecution

# Class: ShellExecution

["@codearts/plugin"](../modules/_codearts_plugin_.md).ShellExecution

## Table of contents

### Constructors

- [constructor](codearts_plugin_.ShellExecution.md#constructor)

### Properties

- [args](codearts_plugin_.ShellExecution.md#args)
- [command](codearts_plugin_.ShellExecution.md#command)
- [commandLine](codearts_plugin_.ShellExecution.md#commandline)
- [options](codearts_plugin_.ShellExecution.md#options)

## Constructors

### constructor

• **new ShellExecution**(`commandLine`, `options?`)

Creates a shell execution with a full command line.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `commandLine` | `string` | The command line to execute. |
| `options?` | [`ShellExecutionOptions`](../interfaces/codearts_plugin_.ShellExecutionOptions.md) | Optional options for the started the shell. |

#### Defined in

[index.d.ts:7534](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7534)

• **new ShellExecution**(`command`, `args`, `options?`)

Creates a shell execution with a command and arguments. For the real execution the editor will
construct a command line from the command and the arguments. This is subject to interpretation
especially when it comes to quoting. If full control over the command line is needed please
use the constructor that creates a `ShellExecution` with the full command line.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `command` | `string` \| [`ShellQuotedString`](../interfaces/codearts_plugin_.ShellQuotedString.md) | The command to execute. |
| `args` | (`string` \| [`ShellQuotedString`](../interfaces/codearts_plugin_.ShellQuotedString.md))[] | The command arguments. |
| `options?` | [`ShellExecutionOptions`](../interfaces/codearts_plugin_.ShellExecutionOptions.md) | Optional options for the started the shell. |

#### Defined in

[index.d.ts:7546](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7546)

## Properties

### args

• **args**: (`string` \| [`ShellQuotedString`](../interfaces/codearts_plugin_.ShellQuotedString.md))[]

The shell args. Is `undefined` if created with a full command line.

#### Defined in

[index.d.ts:7561](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7561)

___

### command

• **command**: `string` \| [`ShellQuotedString`](../interfaces/codearts_plugin_.ShellQuotedString.md)

The shell command. Is `undefined` if created with a full command line.

#### Defined in

[index.d.ts:7556](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7556)

___

### commandLine

• **commandLine**: `undefined` \| `string`

The shell command line. Is `undefined` if created with a command and arguments.

#### Defined in

[index.d.ts:7551](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7551)

___

### options

• `Optional` **options**: [`ShellExecutionOptions`](../interfaces/codearts_plugin_.ShellExecutionOptions.md)

The shell options used when the command line is executed in a shell.
Defaults to undefined.

#### Defined in

[index.d.ts:7567](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7567)
