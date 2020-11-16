**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CustomExecution

# Class: CustomExecution

Class used to execute an extension callback as a task.

## Hierarchy

* **CustomExecution**

## Index

### Constructors

* [constructor](_index_d_._plugin_.customexecution.md#constructor)

## Constructors

### constructor

\+ **new CustomExecution**(`callback`: () => [Thenable](../interfaces/_index_d_.thenable.md)\<[Pseudoterminal](../interfaces/_index_d_._plugin_.pseudoterminal.md)>): [CustomExecution](_index_d_._plugin_.customexecution.md)

*Defined in [index.d.ts:5909](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5909)*

Constructs a CustomExecution task object. The callback will be executed the task is run, at which point the
extension should return the Pseudoterminal it will "run in". The task should wait to do further execution until
[Pseudoterminal.open](#Pseudoterminal.open) is called. Task cancellation should be handled using
[Pseudoterminal.close](#Pseudoterminal.close). When the task is complete fire
[Pseudoterminal.onDidClose](#Pseudoterminal.onDidClose).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`callback` | () => [Thenable](../interfaces/_index_d_.thenable.md)\<[Pseudoterminal](../interfaces/_index_d_._plugin_.pseudoterminal.md)> | The callback that will be called when the task is started by a user.  |

**Returns:** [CustomExecution](_index_d_._plugin_.customexecution.md)
