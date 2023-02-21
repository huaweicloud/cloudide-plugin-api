[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](_cloudide_plugin_.md) / tasks

# Namespace: tasks

["@cloudide/plugin"](_cloudide_plugin_.md).tasks

## Table of contents

### Variables

- [taskExecutions](cloudide_plugin_.tasks.md#taskexecutions)

### Functions

- [executeTask](cloudide_plugin_.tasks.md#executetask)
- [fetchTasks](cloudide_plugin_.tasks.md#fetchtasks)
- [onDidEndTask](cloudide_plugin_.tasks.md#ondidendtask)
- [onDidEndTaskProcess](cloudide_plugin_.tasks.md#ondidendtaskprocess)
- [onDidStartTask](cloudide_plugin_.tasks.md#ondidstarttask)
- [onDidStartTaskProcess](cloudide_plugin_.tasks.md#ondidstarttaskprocess)
- [registerTaskProvider](cloudide_plugin_.tasks.md#registertaskprovider)

## Variables

### taskExecutions

• `Const` **taskExecutions**: `ReadonlyArray`<[`TaskExecution`](../interfaces/cloudide_plugin_.TaskExecution.md)\>

The currently active task executions or an empty array.

#### Defined in

[index.d.ts:10707](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10707)

## Functions

### executeTask

▸ **executeTask**(`task`): `PromiseLike`<[`TaskExecution`](../interfaces/cloudide_plugin_.TaskExecution.md)\>

Executes a task that is managed by VS Code. The returned
task execution can be used to terminate the task.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | [`Task`](../classes/cloudide_plugin_.Task.md) | the task to execute |

#### Returns

`PromiseLike`<[`TaskExecution`](../interfaces/cloudide_plugin_.TaskExecution.md)\>

#### Defined in

[index.d.ts:10702](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10702)

___

### fetchTasks

▸ **fetchTasks**(`filter?`): `PromiseLike`<[`Task`](../classes/cloudide_plugin_.Task.md)[]\>

Fetches all tasks available in the systems. This includes tasks
from `tasks.json` files as well as tasks from task providers
contributed through extensions and plugins.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `filter?` | [`TaskFilter`](../interfaces/cloudide_plugin_.TaskFilter.md) | a filter to filter the return tasks. |

#### Returns

`PromiseLike`<[`Task`](../classes/cloudide_plugin_.Task.md)[]\>

#### Defined in

[index.d.ts:10694](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10694)

___

### onDidEndTask

▸ **onDidEndTask**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TaskEndEvent`](../interfaces/cloudide_plugin_.TaskEndEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidEndTaskProcess

▸ **onDidEndTaskProcess**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TaskProcessEndEvent`](../interfaces/cloudide_plugin_.TaskProcessEndEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidStartTask

▸ **onDidStartTask**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TaskStartEvent`](../interfaces/cloudide_plugin_.TaskStartEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### onDidStartTaskProcess

▸ **onDidStartTaskProcess**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`TaskProcessStartEvent`](../interfaces/cloudide_plugin_.TaskProcessStartEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### registerTaskProvider

▸ **registerTaskProvider**(`type`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a task provider.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | The task kind type this provider is registered for. |
| `provider` | [`TaskProvider`](../interfaces/cloudide_plugin_.TaskProvider.md)<[`Task`](../classes/cloudide_plugin_.Task.md)\> | A task provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:10685](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10685)
