[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ShellExecutionOptions

# Interface: ShellExecutionOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ShellExecutionOptions

## Table of contents

### Properties

- [cwd](cloudide_plugin_.ShellExecutionOptions.md#cwd)
- [env](cloudide_plugin_.ShellExecutionOptions.md#env)
- [executable](cloudide_plugin_.ShellExecutionOptions.md#executable)
- [shellArgs](cloudide_plugin_.ShellExecutionOptions.md#shellargs)
- [shellQuoting](cloudide_plugin_.ShellExecutionOptions.md#shellquoting)

## Properties

### cwd

• `Optional` **cwd**: `string`

The current working directory of the executed shell.
If omitted the tools current workspace root is used.

#### Defined in

[index.d.ts:10259](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10259)

___

### env

• `Optional` **env**: `Object`

The additional environment of the executed shell. If omitted
the parent process' environment is used. If provided it is merged with
the parent process' environment.

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

[index.d.ts:10266](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10266)

___

### executable

• `Optional` **executable**: `string`

The shell executable

#### Defined in

[index.d.ts:10242](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10242)

___

### shellArgs

• `Optional` **shellArgs**: `string`[]

The arguments to be passed to the shell executable used to run the task. Most shells
require special arguments to execute a command. For  example `bash` requires the `-c`
argument to execute a command, `PowerShell` requires `-Command` and `cmd` requires both
`/d` and `/c`.

#### Defined in

[index.d.ts:10250](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10250)

___

### shellQuoting

• `Optional` **shellQuoting**: [`ShellQuotingOptions`](cloudide_plugin_.ShellQuotingOptions.md)

The shell quotes supported by this shell

#### Defined in

[index.d.ts:10253](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10253)
