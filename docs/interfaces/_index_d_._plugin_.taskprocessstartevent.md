**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TaskProcessStartEvent

# Interface: TaskProcessStartEvent

An event signaling the start of a process execution
triggered through a task

## Hierarchy

* **TaskProcessStartEvent**

## Index

### Properties

* [execution](_index_d_._plugin_.taskprocessstartevent.md#execution)
* [processId](_index_d_._plugin_.taskprocessstartevent.md#processid)

## Properties

### execution

• `Readonly` **execution**: [TaskExecution](_index_d_._plugin_.taskexecution.md)

*Defined in [index.d.ts:6116](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6116)*

The task execution for which the process got started.

___

### processId

• `Readonly` **processId**: number

*Defined in [index.d.ts:6121](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6121)*

The underlying process id.
