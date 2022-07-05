[@codearts/plugin](../README.md) / Thenable

# Interface: Thenable<T\>

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Methods

- [then](Thenable.md#then)

## Methods

### then

▸ **then**<`TResult`\>(`onfulfilled?`, `onrejected?`): [`Thenable`](Thenable.md)<`TResult`\>

#### Type parameters

| Name |
| :------ |
| `TResult` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `onfulfilled?` | (`value`: `T`) => `TResult` \| [`Thenable`](Thenable.md)<`TResult`\> |  |
| `onrejected?` | (`reason`: `any`) => `TResult` \| [`Thenable`](Thenable.md)<`TResult`\> |  |

#### Returns

[`Thenable`](Thenable.md)<`TResult`\>

#### Defined in

[index.d.ts:16120](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L16120)

▸ **then**<`TResult`\>(`onfulfilled?`, `onrejected?`): [`Thenable`](Thenable.md)<`TResult`\>

#### Type parameters

| Name |
| :------ |
| `TResult` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `onfulfilled?` | (`value`: `T`) => `TResult` \| [`Thenable`](Thenable.md)<`TResult`\> |
| `onrejected?` | (`reason`: `any`) => `void` |

#### Returns

[`Thenable`](Thenable.md)<`TResult`\>

#### Defined in

[index.d.ts:16121](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L16121)
