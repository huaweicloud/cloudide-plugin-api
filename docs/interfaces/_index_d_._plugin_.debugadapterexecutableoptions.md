**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugAdapterExecutableOptions

# Interface: DebugAdapterExecutableOptions

Options for a debug adapter executable.

## Hierarchy

* **DebugAdapterExecutableOptions**

## Index

### Properties

* [cwd](_index_d_._plugin_.debugadapterexecutableoptions.md#cwd)
* [env](_index_d_._plugin_.debugadapterexecutableoptions.md#env)

## Properties

### cwd

• `Optional` **cwd**: string

*Defined in [index.d.ts:11671](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11671)*

The current working directory for the executed debug adapter.

___

### env

• `Optional` **env**: { [key:string]: string;  }

*Defined in [index.d.ts:11666](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11666)*

The additional environment of the executed program or shell. If omitted
the parent process' environment is used. If provided it is merged with
the parent process' environment.
