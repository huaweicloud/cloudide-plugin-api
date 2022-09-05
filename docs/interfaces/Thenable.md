[@codearts/plugin](../README.md) / Thenable

# Interface: Thenable<T\>

Thenable is a common denominator between ES6 promises, Q, jquery.Deferred, WinJS.Promise,
and others. This API makes no assumption about what promise library is being used which
enables reusing existing code without migrating to a specific promise implementation. Still,
we recommend the use of native promises which are available in this editor.

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

Attaches callbacks for the resolution and/or rejection of the Promise.

#### Type parameters

| Name |
| :------ |
| `TResult` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `onfulfilled?` | (`value`: `T`) => `TResult` \| [`Thenable`](Thenable.md)<`TResult`\> | The callback to execute when the Promise is resolved. |
| `onrejected?` | (`reason`: `any`) => `TResult` \| [`Thenable`](Thenable.md)<`TResult`\> | The callback to execute when the Promise is rejected. |

#### Returns

[`Thenable`](Thenable.md)<`TResult`\>

A Promise for the completion of which ever callback is executed.

#### Defined in

[index.d.ts:16212](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L16212)

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

[index.d.ts:16213](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L16213)
