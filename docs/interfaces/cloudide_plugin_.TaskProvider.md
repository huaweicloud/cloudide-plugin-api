[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TaskProvider

# Interface: TaskProvider<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TaskProvider

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`Task`](../classes/cloudide_plugin_.Task.md) = [`Task`](../classes/cloudide_plugin_.Task.md) |

## Table of contents

### Methods

- [provideTasks](cloudide_plugin_.TaskProvider.md#providetasks)
- [resolveTask](cloudide_plugin_.TaskProvider.md#resolvetask)

## Methods

### provideTasks

▸ **provideTasks**(`token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`[]\>

Provides tasks.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`[]\>

an array of tasks

#### Defined in

[index.d.ts:10573](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10573)

___

### resolveTask

▸ **resolveTask**(`task`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`\>

Resolves a task that has no [`execution`](#Task.execution) set. Tasks are
often created from information found in the `tasks.json`-file. Such tasks miss
the information on how to execute them and a task provider must fill in
the missing information in the `resolveTask`-method.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | `T` | The task to resolve. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`\>

The resolved task

#### Defined in

[index.d.ts:10585](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10585)
