[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ProcessExecutionOptions

# Interface: ProcessExecutionOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).ProcessExecutionOptions

Options for a process execution

## Table of contents

### Properties

- [cwd](codearts_plugin_.ProcessExecutionOptions.md#cwd)
- [env](codearts_plugin_.ProcessExecutionOptions.md#env)

## Properties

### cwd

• `Optional` **cwd**: `string`

The current working directory of the executed program or shell.
If omitted the tools current workspace root is used.

#### Defined in

[index.d.ts:7363](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7363)

___

### env

• `Optional` **env**: `Object`

The additional environment of the executed program or shell. If omitted
the parent process' environment is used. If provided it is merged with
the parent process' environment.

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

[index.d.ts:7370](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7370)
