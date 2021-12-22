**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TaskProvider

# Interface: TaskProvider\<T>

A task provider allows to add tasks to the task service.
A task provider is registered via #tasks.registerTaskProvider.

## Type parameters

Name | Type | Default |
------ | ------ | ------ |
`T` | [Task](../classes/_index_d_._plugin_.task.md) | Task |

## Hierarchy

* **TaskProvider**

## Index

### Methods

* [provideTasks](_index_d_._plugin_.taskprovider.md#providetasks)
* [resolveTask](_index_d_._plugin_.taskprovider.md#resolvetask)

## Methods

### provideTasks

▸ **provideTasks**(`token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T[]>

*Defined in [index.d.ts:6655](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6655)*

Provides tasks.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T[]>

an array of tasks

___

### resolveTask

▸ **resolveTask**(`task`: T, `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T>

*Defined in [index.d.ts:6670](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L6670)*

Resolves a task that has no [`execution`](#Task.execution) set. Tasks are
often created from information found in the `tasks.json`-file. Such tasks miss
the information on how to execute them and a task provider must fill in
the missing information in the `resolveTask`-method. This method will not be
called for tasks returned from the above `provideTasks` method since those
tasks are always fully resolved. A valid default implementation for the
`resolveTask` method is to return `undefined`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`task` | T | The task to resolve. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T>

The resolved task
