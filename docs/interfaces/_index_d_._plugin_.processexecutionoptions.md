**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ProcessExecutionOptions

# Interface: ProcessExecutionOptions

Options for a process execution

## Hierarchy

* **ProcessExecutionOptions**

## Index

### Properties

* [cwd](_index_d_._plugin_.processexecutionoptions.md#cwd)
* [env](_index_d_._plugin_.processexecutionoptions.md#env)

## Properties

### cwd

• `Optional` **cwd**: string

*Defined in [index.d.ts:5699](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5699)*

The current working directory of the executed program or shell.
If omitted the tools current workspace root is used.

___

### env

• `Optional` **env**: { [key:string]: string;  }

*Defined in [index.d.ts:5706](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5706)*

The additional environment of the executed program or shell. If omitted
the parent process' environment is used. If provided it is merged with
the parent process' environment.
