**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TerminalOptions

# Interface: TerminalOptions

Value-object describing what options a terminal should use.

## Hierarchy

* **TerminalOptions**

## Index

### Properties

* [cwd](_index_d_._plugin_.terminaloptions.md#cwd)
* [env](_index_d_._plugin_.terminaloptions.md#env)
* [hideFromUser](_index_d_._plugin_.terminaloptions.md#hidefromuser)
* [name](_index_d_._plugin_.terminaloptions.md#name)
* [shellArgs](_index_d_._plugin_.terminaloptions.md#shellargs)
* [shellPath](_index_d_._plugin_.terminaloptions.md#shellpath)
* [strictEnv](_index_d_._plugin_.terminaloptions.md#strictenv)

## Properties

### cwd

• `Optional` **cwd**: string \| [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:8093](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8093)*

A path or Uri for the current working directory to be used for the terminal.

___

### env

• `Optional` **env**: { [key:string]: string \| null;  }

*Defined in [index.d.ts:8098](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8098)*

Object with environment variables that will be added to the VS Code process.

___

### hideFromUser

• `Optional` **hideFromUser**: boolean

*Defined in [index.d.ts:8116](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8116)*

When enabled the terminal will run the process as normal but not be surfaced to the user
until `Terminal.show` is called. The typical usage for this is when you need to run
something that may need interactivity but only want to tell the user about it when
interaction is needed. Note that the terminals will still be exposed to all extensions
as normal.

___

### name

• `Optional` **name**: string

*Defined in [index.d.ts:8077](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8077)*

A human-readable string which will be used to represent the terminal in the UI.

___

### shellArgs

• `Optional` **shellArgs**: string[] \| string

*Defined in [index.d.ts:8088](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8088)*

Args for the custom shell executable. A string can be used on Windows only which allows
specifying shell args in [command-line format](https://msdn.microsoft.com/en-au/08dfcab2-eb6e-49a4-80eb-87d4076c98c6).

___

### shellPath

• `Optional` **shellPath**: string

*Defined in [index.d.ts:8082](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8082)*

A path to a custom shell executable to be used in the terminal.

___

### strictEnv

• `Optional` **strictEnv**: boolean

*Defined in [index.d.ts:8107](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8107)*

Whether the terminal process environment should be exactly as provided in
`TerminalOptions.env`. When this is false (default), the environment will be based on the
window's environment and also apply configured platform settings like
`terminal.integrated.windows.env` on top. When this is true, the complete environment
must be provided as nothing will be inherited from the process or any configuration.
