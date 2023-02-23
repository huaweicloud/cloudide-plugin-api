[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](_cloudide_plugin_.md) / extensions

# Namespace: extensions

["@cloudide/plugin"](_cloudide_plugin_.md).extensions

## Table of contents

### Variables

- [all](cloudide_plugin_.extensions.md#all)

### Functions

- [getExtension](cloudide_plugin_.extensions.md#getextension)
- [onDidChange](cloudide_plugin_.extensions.md#ondidchange)

## Variables

### all

• **all**: [`Extension`](../interfaces/cloudide_plugin_.Extension.md)<`any`\>[]

All plug-ins currently known to the system.

#### Defined in

[index.d.ts:238](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L238)

## Functions

### getExtension

▸ **getExtension**(`pluginId`): [`Extension`](../interfaces/cloudide_plugin_.Extension.md)<`any`\> \| `undefined`

Get an plug-in by its full identifier in the form of: `publisher.name`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pluginId` | `string` | An plug-in identifier. |

#### Returns

[`Extension`](../interfaces/cloudide_plugin_.Extension.md)<`any`\> \| `undefined`

An plug-in or `undefined`.

#### Defined in

[index.d.ts:225](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L225)

▸ **getExtension**<`T`\>(`pluginId`): [`Extension`](../interfaces/cloudide_plugin_.Extension.md)<`T`\> \| `undefined`

Get an plug-in its full identifier in the form of: `publisher.name`.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pluginId` | `string` | An plug-in identifier. |

#### Returns

[`Extension`](../interfaces/cloudide_plugin_.Extension.md)<`T`\> \| `undefined`

An plug-in or `undefined`.

#### Defined in

[index.d.ts:233](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L233)

___

### onDidChange

▸ **onDidChange**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: `void`) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)
