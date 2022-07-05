[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TaskProvider

# Interface: TaskProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).TaskProvider

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

#### Defined in

[index.d.ts:7591](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L7591)

___

### resolveTask

▸ **resolveTask**(`task`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | `T` |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Defined in

[index.d.ts:7610](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L7610)
