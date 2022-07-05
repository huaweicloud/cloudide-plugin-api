[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Event

# Interface: Event<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).Event

## Type parameters

| Name |
| :------ |
| `T` |

## Callable

### Event

▸ **Event**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: `T`) => `any` |  |
| `thisArgs?` | `any` |  |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L1603)
