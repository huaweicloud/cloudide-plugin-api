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

*Defined in [index.d.ts:6810](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6810)*

Fires when a task ends.

___

### onDidEndTaskProcess

• `Const` **onDidEndTaskProcess**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TaskProcessEndEvent](../interfaces/_index_d_._plugin_.taskprocessendevent.md)>

*Defined in [index.d.ts:6824](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6824)*

Fires when the underlying process has ended.
This event will not fire for tasks that don't
execute an underlying process.

___

### onDidStartTask

• `Const` **onDidStartTask**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TaskStartEvent](../interfaces/_index_d_._plugin_.taskstartevent.md)>

*Defined in [index.d.ts:6805](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6805)*

Fires when a task starts.

___

### onDidStartTaskProcess

• `Const` **onDidStartTaskProcess**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[TaskProcessStartEvent](../interfaces/_index_d_._plugin_.taskprocessstartevent.md)>

*Defined in [index.d.ts:6817](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6817)*

Fires when the underlying process has been started.
This event will not fire for tasks that don't
execute an underlying process.

___

### taskExecutions

• `Const` **taskExecutions**: ReadonlyArray\<[TaskExecution](../interfaces/_index_d_._plugin_.taskexecution.md)>

*Defined in [index.d.ts:6800](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6800)*

The currently active task executions or an empty array.

## Functions

### executeTask

▸ **executeTask**(`task`: [Task](../classes/_index_d_._plugin_.task.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<[TaskExecution](../interfaces/_index_d_._plugin_.taskexecution.md)>

*Defined in [index.d.ts:6795](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6795)*

Executes a task that is managed by VS Code. The returned
task execution can be used to terminate the task.

**`throws`** When running a ShellExecution or a ProcessExecution
task in an environment where a new process cannot be started.
In such an environment, only CustomExecution tasks can be run.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`task` | [Task](../classes/_index_d_._plugin_.task.md) | the task to execute  |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[TaskExecution](../interfaces/_index_d_._plugin_.taskexecution.md)>

___

### fetchTasks

▸ **fetchTasks**(`filter?`: [TaskFilter](../interfaces/_index_d_._plugin_.taskfilter.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<[Task](../classes/_index_d_._plugin_.task.md)[]>

*Defined in [index.d.ts:6783](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6783)*

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

*Defined in [index.d.ts:6774](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6774)*

Register a task provider.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`type` | string | The task kind type this provider is registered for. |
`provider` | [TaskProvider](../interfaces/_index_d_._plugin_.taskprovider.md) | A task provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.
