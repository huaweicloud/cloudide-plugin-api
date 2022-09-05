[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TaskProvider

# Interface: TaskProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).TaskProvider

A task provider allows to add tasks to the task service.
A task provider is registered via [registerTaskProvider](../modules/codearts_plugin_.tasks.md#registertaskprovider).

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`Task`](../classes/codearts_plugin_.Task.md) = [`Task`](../classes/codearts_plugin_.Task.md) |

## Table of contents

### Methods

- [provideTasks](codearts_plugin_.TaskProvider.md#providetasks)
- [resolveTask](codearts_plugin_.TaskProvider.md#resolvetask)

## Methods

### provideTasks

▸ **provideTasks**(`token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

Provides tasks.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

an array of tasks

#### Defined in

[index.d.ts:7591](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7591)

___

### resolveTask

▸ **resolveTask**(`task`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

Resolves a task that has no [`execution`](../classes/codearts_plugin_.Task.md#execution) set. Tasks are
often created from information found in the `tasks.json`-file. Such tasks miss
the information on how to execute them and a task provider must fill in
the missing information in the `resolveTask`-method. This method will not be
called for tasks returned from the above `provideTasks` method since those
tasks are always fully resolved. A valid default implementation for the
`resolveTask` method is to return `undefined`.

Note that when filling in the properties of `task`, you _must_ be sure to
use the exact same `TaskDefinition` and not create a new one. Other properties
may be changed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | `T` | The task to resolve. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

The resolved task

#### Defined in

[index.d.ts:7610](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7610)
