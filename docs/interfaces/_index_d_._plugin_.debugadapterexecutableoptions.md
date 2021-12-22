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

*Defined in [index.d.ts:11703](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11703)*

The current working directory for the executed debug adapter.

___

### env

• `Optional` **env**: { [key:string]: string;  }

*Defined in [index.d.ts:11698](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11698)*

The additional environment of the executed program or shell. If omitted
the parent process' environment is used. If provided it is merged with
the parent process' environment.
