[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ShellExecutionOptions

# Interface: ShellExecutionOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).ShellExecutionOptions

Options for a shell execution

## Table of contents

### Properties

- [cwd](codearts_plugin_.ShellExecutionOptions.md#cwd)
- [env](codearts_plugin_.ShellExecutionOptions.md#env)
- [executable](codearts_plugin_.ShellExecutionOptions.md#executable)
- [shellArgs](codearts_plugin_.ShellExecutionOptions.md#shellargs)
- [shellQuoting](codearts_plugin_.ShellExecutionOptions.md#shellquoting)

## Properties

### cwd

• `Optional` **cwd**: `string`

The current working directory of the executed shell.
If omitted the tools current workspace root is used.

#### Defined in

[index.d.ts:7369](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7369)

___

### env

• `Optional` **env**: `Object`

The additional environment of the executed shell. If omitted
the parent process' environment is used. If provided it is merged with
the parent process' environment.

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

[index.d.ts:7376](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7376)

___

### executable

• `Optional` **executable**: `string`

The shell executable.

#### Defined in

[index.d.ts:7350](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7350)

___

### shellArgs

• `Optional` **shellArgs**: `string`[]

The arguments to be passed to the shell executable used to run the task. Most shells
require special arguments to execute a command. For  example `bash` requires the `-c`
argument to execute a command, `PowerShell` requires `-Command` and `cmd` requires both
`/d` and `/c`.

#### Defined in

[index.d.ts:7358](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7358)

___

### shellQuoting

• `Optional` **shellQuoting**: [`ShellQuotingOptions`](codearts_plugin_.ShellQuotingOptions.md)

The shell quotes supported by this shell.

#### Defined in

[index.d.ts:7363](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7363)
