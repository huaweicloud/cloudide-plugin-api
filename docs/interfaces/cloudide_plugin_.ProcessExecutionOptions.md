[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ProcessExecutionOptions

# Interface: ProcessExecutionOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ProcessExecutionOptions

## Table of contents

### Properties

- [cwd](cloudide_plugin_.ProcessExecutionOptions.md#cwd)
- [env](cloudide_plugin_.ProcessExecutionOptions.md#env)

## Properties

### cwd

• `Optional` **cwd**: `string`

The current working directory of the executed program or shell.
If omitted the tools current workspace root is used.

#### Defined in

[index.d.ts:10317](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10317)

___

### env

• `Optional` **env**: `Object`

The additional environment of the executed program or shell. If omitted
the parent process' environment is used. If provided it is merged with
the parent process' environment.

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

[index.d.ts:10324](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10324)
