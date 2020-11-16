**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ProcessExecution

# Class: ProcessExecution

The execution of a task happens as an external process
without shell interaction.

## Hierarchy

* **ProcessExecution**

## Index

### Constructors

* [constructor](_index_d_._plugin_.processexecution.md#constructor)

### Properties

* [args](_index_d_._plugin_.processexecution.md#args)
* [options](_index_d_._plugin_.processexecution.md#options)
* [process](_index_d_._plugin_.processexecution.md#process)

## Constructors

### constructor

\+ **new ProcessExecution**(`process`: string, `options?`: [ProcessExecutionOptions](../interfaces/_index_d_._plugin_.processexecutionoptions.md)): [ProcessExecution](_index_d_._plugin_.processexecution.md)

*Defined in [index.d.ts:5713](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5713)*

Creates a process execution.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`process` | string | The process to start. |
`options?` | [ProcessExecutionOptions](../interfaces/_index_d_._plugin_.processexecutionoptions.md) | Optional options for the started process.  |

**Returns:** [ProcessExecution](_index_d_._plugin_.processexecution.md)

\+ **new ProcessExecution**(`process`: string, `args`: string[], `options?`: [ProcessExecutionOptions](../interfaces/_index_d_._plugin_.processexecutionoptions.md)): [ProcessExecution](_index_d_._plugin_.processexecution.md)

*Defined in [index.d.ts:5721](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5721)*

Creates a process execution.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`process` | string | The process to start. |
`args` | string[] | Arguments to be passed to the process. |
`options?` | [ProcessExecutionOptions](../interfaces/_index_d_._plugin_.processexecutionoptions.md) | Optional options for the started process.  |

**Returns:** [ProcessExecution](_index_d_._plugin_.processexecution.md)

## Properties

### args

•  **args**: string[]

*Defined in [index.d.ts:5740](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5740)*

The arguments passed to the process. Defaults to an empty array.

___

### options

• `Optional` **options**: [ProcessExecutionOptions](../interfaces/_index_d_._plugin_.processexecutionoptions.md)

*Defined in [index.d.ts:5746](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5746)*

The process options used when the process is executed.
Defaults to undefined.

___

### process

•  **process**: string

*Defined in [index.d.ts:5735](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5735)*

The process to be executed.
