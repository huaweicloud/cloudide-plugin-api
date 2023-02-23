[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ShellExecution

# Class: ShellExecution

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ShellExecution

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.ShellExecution.md#constructor)

### Properties

- [args](cloudide_plugin_.ShellExecution.md#args)
- [command](cloudide_plugin_.ShellExecution.md#command)
- [commandLine](cloudide_plugin_.ShellExecution.md#commandline)
- [options](cloudide_plugin_.ShellExecution.md#options)

## Constructors

### constructor

• **new ShellExecution**(`commandLine`, `options?`)

Creates a shell execution with a full command line.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `commandLine` | `string` | The command line to execute. |
| `options?` | [`ShellExecutionOptions`](../interfaces/cloudide_plugin_.ShellExecutionOptions.md) | Optional options for the started the shell. |

#### Defined in

[index.d.ts:10276](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10276)

• **new ShellExecution**(`command`, `args`, `options?`)

Creates a shell execution with a command and arguments. For the real execution VS Code will
construct a command line from the command and the arguments. This is subject to interpretation
especially when it comes to quoting. If full control over the command line is needed please
use the constructor that creates a `ShellExecution` with the full command line.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `command` | `string` \| [`ShellQuotedString`](../interfaces/cloudide_plugin_.ShellQuotedString.md) | The command to execute. |
| `args` | (`string` \| [`ShellQuotedString`](../interfaces/cloudide_plugin_.ShellQuotedString.md))[] | The command arguments. |
| `options?` | [`ShellExecutionOptions`](../interfaces/cloudide_plugin_.ShellExecutionOptions.md) | Optional options for the started the shell. |

#### Defined in

[index.d.ts:10288](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10288)

## Properties

### args

• `Optional` **args**: (`string` \| [`ShellQuotedString`](../interfaces/cloudide_plugin_.ShellQuotedString.md))[]

The shell args. Is `undefined` if created with a full command line.

#### Defined in

[index.d.ts:10309](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10309)

___

### command

• `Optional` **command**: `string` \| [`ShellQuotedString`](../interfaces/cloudide_plugin_.ShellQuotedString.md)

The shell command. Is `undefined` if created with a full command line.

#### Defined in

[index.d.ts:10304](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10304)

___

### commandLine

• `Optional` **commandLine**: `string`

The shell command line. Is `undefined` if created with a command and arguments.

#### Defined in

[index.d.ts:10293](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10293)

___

### options

• `Optional` **options**: [`ShellExecutionOptions`](../interfaces/cloudide_plugin_.ShellExecutionOptions.md)

The shell options used when the command line is executed in a shell.
Defaults to undefined.

#### Defined in

[index.d.ts:10299](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10299)
