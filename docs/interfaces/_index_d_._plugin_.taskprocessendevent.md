**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TaskProcessEndEvent

# Interface: TaskProcessEndEvent

An event signaling the end of a process execution
triggered through a task

## Hierarchy

* **TaskProcessEndEvent**

## Index

### Properties

* [execution](_index_d_._plugin_.taskprocessendevent.md#execution)
* [exitCode](_index_d_._plugin_.taskprocessendevent.md#exitcode)

## Properties

### execution

• `Readonly` **execution**: [TaskExecution](_index_d_._plugin_.taskexecution.md)

*Defined in [index.d.ts:6133](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6133)*

The task execution for which the process got started.

___

### exitCode

• `Readonly` **exitCode**: number

*Defined in [index.d.ts:6138](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6138)*

The process's exit code.
