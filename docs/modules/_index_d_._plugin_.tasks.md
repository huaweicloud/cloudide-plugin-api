**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](_index_d_.md) / ["plugin"](_index_d_._plugin_.md) / tasks

# Namespace: tasks

Namespace for tasks functionality.

## Index

### Variables

* [onDidEndTask](_index_d_._plugin_.tasks.md#ondidendtask)
* [onDidEndTaskProcess](_index_d_._plugin_.tasks.md#ondidendtaskprocess)
* [onDidStartTask](_index_d_._plugin_.tasks.md#ondidstarttask)
* [onDidStartTaskProcess](_index_d_._plugin_.tasks.md#ondidstarttaskprocess)
* [taskExecutions](_index_d_._plugin_.tasks.md#taskexecutions)

### Functions

* [executeTask](_index_d_._plugin_.tasks.md#executetask)
* [fetchTasks](_index_d_._plugin_.tasks.md#fetchtasks)
* [registerTaskProvider](_index_d_._plugin_.tasks.md#registertaskprovider)

## Variables

### onDidEndTask

• `Const` **onDidEndTask**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TaskEndEvent](../interfaces/_index_d_._plugin_.taskendevent.md)>

*Defined in [index.d.ts:6198](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6198)*

Fires when a task ends.

___

### onDidEndTaskProcess

• `Const` **onDidEndTaskProcess**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TaskProcessEndEvent](../interfaces/_index_d_._plugin_.taskprocessendevent.md)>

*Defined in [index.d.ts:6212](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6212)*

Fires when the underlying process has ended.
This event will not fire for tasks that don't
execute an underlying process.

___

### onDidStartTask

• `Const` **onDidStartTask**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TaskStartEvent](../interfaces/_index_d_._plugin_.taskstartevent.md)>

*Defined in [index.d.ts:6193](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6193)*

Fires when a task starts.

___

### onDidStartTaskProcess

• `Const` **onDidStartTaskProcess**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TaskProcessStartEvent](../interfaces/_index_d_._plugin_.taskprocessstartevent.md)>

*Defined in [index.d.ts:6205](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6205)*

Fires when the underlying process has been started.
This event will not fire for tasks that don't
execute an underlying process.

___

### taskExecutions

• `Const` **taskExecutions**: ReadonlyArray\<[TaskExecution](../interfaces/_index_d_._plugin_.taskexecution.md)>

*Defined in [index.d.ts:6188](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6188)*

The currently active task executions or an empty array.

## Functions

### executeTask

▸ **executeTask**(`task`: [Task](../classes/_index_d_._plugin_.task.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<[TaskExecution](../interfaces/_index_d_._plugin_.taskexecution.md)>

*Defined in [index.d.ts:6183](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6183)*

Executes a task that is managed by VS Code. The returned
task execution can be used to terminate the task.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`task` | [Task](../classes/_index_d_._plugin_.task.md) | the task to execute  |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[TaskExecution](../interfaces/_index_d_._plugin_.taskexecution.md)>

___

### fetchTasks

▸ **fetchTasks**(`filter?`: [TaskFilter](../interfaces/_index_d_._plugin_.taskfilter.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<[Task](../classes/_index_d_._plugin_.task.md)[]>

*Defined in [index.d.ts:6175](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6175)*

Fetches all tasks available in the systems. This includes tasks
from `tasks.json` files as well as tasks from task providers
contributed through extensions.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`filter?` | [TaskFilter](../interfaces/_index_d_._plugin_.taskfilter.md) | Optional filter to select tasks of a certain type or version.  |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[Task](../classes/_index_d_._plugin_.task.md)[]>

___

### registerTaskProvider

▸ **registerTaskProvider**(`type`: string, `provider`: [TaskProvider](../interfaces/_index_d_._plugin_.taskprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:6166](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6166)*

Register a task provider.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`type` | string | The task kind type this provider is registered for. |
`provider` | [TaskProvider](../interfaces/_index_d_._plugin_.taskprovider.md) | A task provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.
