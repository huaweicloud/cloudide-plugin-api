[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / extensions

# Namespace: extensions

["@codearts/plugin"](_codearts_plugin_.md).extensions

## Table of contents

### Variables

- [all](codearts_plugin_.extensions.md#all)

### Functions

- [getExtension](codearts_plugin_.extensions.md#getextension)
- [onDidChange](codearts_plugin_.extensions.md#ondidchange)

## Variables

### all

• **all**: readonly [`Extension`](../interfaces/codearts_plugin_.Extension.md)<`any`\>[]

#### Defined in

[index.d.ts:14701](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14701)

## Functions

### getExtension

▸ **getExtension**<`T`\>(`extensionId`): [`Extension`](../interfaces/codearts_plugin_.Extension.md)<`T`\> \| `undefined`

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `any` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `extensionId` | `string` |  |

#### Returns

[`Extension`](../interfaces/codearts_plugin_.Extension.md)<`T`\> \| `undefined`

#### Defined in

[index.d.ts:14696](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14696)

___

### onDidChange

▸ `Const` **onDidChange**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: `void`) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:14707](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14707)
