[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DebugAdapterExecutableOptions

# Interface: DebugAdapterExecutableOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DebugAdapterExecutableOptions

Options for a debug adapter executable.

## Table of contents

### Properties

- [cwd](cloudide_plugin_.DebugAdapterExecutableOptions.md#cwd)
- [env](cloudide_plugin_.DebugAdapterExecutableOptions.md#env)

## Properties

### cwd

• `Optional` **cwd**: `string`

The current working directory for the executed debug adapter.

#### Defined in

[index.d.ts:9812](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9812)

___

### env

• `Optional` **env**: `Object`

The additional environment of the executed program or shell. If omitted
the parent process' environment is used. If provided it is merged with
the parent process' environment.

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

[index.d.ts:9807](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9807)
