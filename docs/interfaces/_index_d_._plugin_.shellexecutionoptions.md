**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ShellExecutionOptions

# Interface: ShellExecutionOptions

Options for a shell execution

## Hierarchy

* **ShellExecutionOptions**

## Index

### Properties

* [cwd](_index_d_._plugin_.shellexecutionoptions.md#cwd)
* [env](_index_d_._plugin_.shellexecutionoptions.md#env)
* [executable](_index_d_._plugin_.shellexecutionoptions.md#executable)
* [shellArgs](_index_d_._plugin_.shellexecutionoptions.md#shellargs)
* [shellQuoting](_index_d_._plugin_.shellexecutionoptions.md#shellquoting)

## Properties

### cwd

• `Optional` **cwd**: string

*Defined in [index.d.ts:6405](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6405)*

The current working directory of the executed shell.
If omitted the tools current workspace root is used.

___

### env

• `Optional` **env**: { [key:string]: string;  }

*Defined in [index.d.ts:6412](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6412)*

The additional environment of the executed shell. If omitted
the parent process' environment is used. If provided it is merged with
the parent process' environment.

___

### executable

• `Optional` **executable**: string

*Defined in [index.d.ts:6386](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6386)*

The shell executable.

___

### shellArgs

• `Optional` **shellArgs**: string[]

*Defined in [index.d.ts:6394](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6394)*

The arguments to be passed to the shell executable used to run the task. Most shells
require special arguments to execute a command. For  example `bash` requires the `-c`
argument to execute a command, `PowerShell` requires `-Command` and `cmd` requires both
`/d` and `/c`.

___

### shellQuoting

• `Optional` **shellQuoting**: [ShellQuotingOptions](_index_d_._plugin_.shellquotingoptions.md)

*Defined in [index.d.ts:6399](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6399)*

The shell quotes supported by this shell.
