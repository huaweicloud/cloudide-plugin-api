[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugAdapterExecutableOptions

# Interface: DebugAdapterExecutableOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugAdapterExecutableOptions

Options for a debug adapter executable.

## Table of contents

### Properties

- [cwd](codearts_plugin_.DebugAdapterExecutableOptions.md#cwd)
- [env](codearts_plugin_.DebugAdapterExecutableOptions.md#env)

## Properties

### cwd

• `Optional` **cwd**: `string`

The current working directory for the executed debug adapter.

#### Defined in

[index.d.ts:15220](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15220)

___

### env

• `Optional` **env**: `Object`

The additional environment of the executed program or shell. If omitted
the parent process' environment is used. If provided it is merged with
the parent process' environment.

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

[index.d.ts:15215](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15215)
