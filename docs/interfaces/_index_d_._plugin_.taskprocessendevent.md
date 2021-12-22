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

*Defined in [index.d.ts:6741](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6741)*

The task execution for which the process got started.

___

### exitCode

• `Readonly` **exitCode**: number \| undefined

*Defined in [index.d.ts:6746](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6746)*

The process's exit code. Will be `undefined` when the task is terminated.
