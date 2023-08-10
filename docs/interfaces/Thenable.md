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

[index.d.ts:17986](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17986)

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

[index.d.ts:17987](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L17987)
