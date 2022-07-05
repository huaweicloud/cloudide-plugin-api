[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / tasks

# Namespace: tasks

["@codearts/plugin"](_codearts_plugin_.md).tasks

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

• **taskExecutions**: readonly [`TaskExecution`](../interfaces/codearts_plugin_.TaskExecution.md)[]

#### Defined in

[index.d.ts:7740](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L7740)

## Functions

### executeTask

▸ **executeTask**(`task`): [`Thenable`](../interfaces/Thenable.md)<[`TaskExecution`](../interfaces/codearts_plugin_.TaskExecution.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | [`Task`](../classes/codearts_plugin_.Task.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TaskExecution`](../interfaces/codearts_plugin_.TaskExecution.md)\>

#### Defined in

[index.d.ts:7735](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L7735)

___

### fetchTasks

▸ **fetchTasks**(`filter?`): [`Thenable`](../interfaces/Thenable.md)<[`Task`](../classes/codearts_plugin_.Task.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `filter?` | [`TaskFilter`](../interfaces/codearts_plugin_.TaskFilter.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`Task`](../classes/codearts_plugin_.Task.md)[]\>

#### Defined in

[index.d.ts:7723](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L7723)

___

### onDidEndTask

▸ `Const` **onDidEndTask**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`TaskEndEvent`](../interfaces/codearts_plugin_.TaskEndEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:7750](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L7750)

___

### onDidEndTaskProcess

▸ `Const` **onDidEndTaskProcess**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`TaskProcessEndEvent`](../interfaces/codearts_plugin_.TaskProcessEndEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:7764](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L7764)

___

### onDidStartTask

▸ `Const` **onDidStartTask**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`TaskStartEvent`](../interfaces/codearts_plugin_.TaskStartEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:7745](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L7745)

___

### onDidStartTaskProcess

▸ `Const` **onDidStartTaskProcess**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`TaskProcessStartEvent`](../interfaces/codearts_plugin_.TaskProcessStartEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:7757](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L7757)

___

### registerTaskProvider

▸ **registerTaskProvider**(`type`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` |  |
| `provider` | [`TaskProvider`](../interfaces/codearts_plugin_.TaskProvider.md)<[`Task`](../classes/codearts_plugin_.Task.md)\> |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:7714](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L7714)
