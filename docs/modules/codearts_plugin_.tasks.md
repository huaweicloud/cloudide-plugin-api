[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / tasks

# Namespace: tasks

["@codearts/plugin"](_codearts_plugin_.md).tasks

Namespace for tasks functionality.

## Table of contents

### Variables

- [taskExecutions](codearts_plugin_.tasks.md#taskexecutions)

### Functions

- [executeTask](codearts_plugin_.tasks.md#executetask)
- [fetchTasks](codearts_plugin_.tasks.md#fetchtasks)
- [onDidEndTask](codearts_plugin_.tasks.md#ondidendtask)
- [onDidEndTaskProcess](codearts_plugin_.tasks.md#ondidendtaskprocess)
- [onDidStartTask](codearts_plugin_.tasks.md#ondidstarttask)
- [onDidStartTaskProcess](codearts_plugin_.tasks.md#ondidstarttaskprocess)
- [registerTaskProvider](codearts_plugin_.tasks.md#registertaskprovider)

## Variables

### taskExecutions

• `Const` **taskExecutions**: readonly [`TaskExecution`](../interfaces/codearts_plugin_.TaskExecution.md)[]

The currently active task executions or an empty array.

#### Defined in

[index.d.ts:7838](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7838)

## Functions

### executeTask

▸ **executeTask**(`task`): [`Thenable`](../interfaces/Thenable.md)<[`TaskExecution`](../interfaces/codearts_plugin_.TaskExecution.md)\>

Executes a task that is managed by the editor. The returned
task execution can be used to terminate the task.

**`Throws`**

When running a ShellExecution or a ProcessExecution
task in an environment where a new process cannot be started.
In such an environment, only CustomExecution tasks can be run.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | [`Task`](../classes/codearts_plugin_.Task.md) | the task to execute |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TaskExecution`](../interfaces/codearts_plugin_.TaskExecution.md)\>

#### Defined in

[index.d.ts:7833](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7833)

___

### fetchTasks

▸ **fetchTasks**(`filter?`): [`Thenable`](../interfaces/Thenable.md)<[`Task`](../classes/codearts_plugin_.Task.md)[]\>

Fetches all tasks available in the systems. This includes tasks
from `tasks.json` files as well as tasks from task providers
contributed through extensions.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `filter?` | [`TaskFilter`](../interfaces/codearts_plugin_.TaskFilter.md) | Optional filter to select tasks of a certain type or version. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`Task`](../classes/codearts_plugin_.Task.md)[]\>

#### Defined in

[index.d.ts:7821](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7821)

___

### onDidEndTask

▸ **onDidEndTask**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TaskEndEvent`](../interfaces/codearts_plugin_.TaskEndEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L1603)

___

### onDidEndTaskProcess

▸ **onDidEndTaskProcess**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TaskProcessEndEvent`](../interfaces/codearts_plugin_.TaskProcessEndEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L1603)

___

### onDidStartTask

▸ **onDidStartTask**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TaskStartEvent`](../interfaces/codearts_plugin_.TaskStartEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L1603)

___

### onDidStartTaskProcess

▸ **onDidStartTaskProcess**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TaskProcessStartEvent`](../interfaces/codearts_plugin_.TaskProcessStartEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L1603)

___

### registerTaskProvider

▸ **registerTaskProvider**(`type`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a task provider.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | The task kind type this provider is registered for. |
| `provider` | [`TaskProvider`](../interfaces/codearts_plugin_.TaskProvider.md)<[`Task`](../classes/codearts_plugin_.Task.md)\> | A task provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:7812](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7812)
