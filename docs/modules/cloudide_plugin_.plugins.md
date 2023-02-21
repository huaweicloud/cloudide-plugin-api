[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](_cloudide_plugin_.md) / plugins

# Namespace: plugins

["@cloudide/plugin"](_cloudide_plugin_.md).plugins

Namespace for dealing with installed plug-ins. Plug-ins are represented
by an [plug-in](#Plugin)-interface which enables reflection on them.

Plug-in writers can provide APIs to other plug-ins by returning their API public
surface from the `start`-call.

```javascript
export function start() {
    let api = {
        sum(a, b) {
            return a + b;
        },
        mul(a, b) {
            return a * b;
        }
    };
    // 'export' public api-surface
    return api;
}
```
```javascript
let mathExt = plugins.getPlugin('genius.math');
let importedApi = mathExt.exports;

console.log(importedApi.mul(42, 1));
```

## Table of contents

### Variables

- [all](cloudide_plugin_.plugins.md#all)

### Functions

- [getPlugin](cloudide_plugin_.plugins.md#getplugin)
- [onDidChange](cloudide_plugin_.plugins.md#ondidchange)

## Variables

### all

• **all**: [`Plugin`](../interfaces/cloudide_plugin_.Plugin.md)<`any`\>[]

All plug-ins currently known to the system.

#### Defined in

[index.d.ts:209](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L209)

## Functions

### getPlugin

▸ **getPlugin**(`pluginId`): [`Plugin`](../interfaces/cloudide_plugin_.Plugin.md)<`any`\> \| `undefined`

Get an plug-in by its full identifier in the form of: `publisher.name`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pluginId` | `string` | An plug-in identifier. |

#### Returns

[`Plugin`](../interfaces/cloudide_plugin_.Plugin.md)<`any`\> \| `undefined`

An plug-in or `undefined`.

#### Defined in

[index.d.ts:196](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L196)

▸ **getPlugin**<`T`\>(`pluginId`): [`Plugin`](../interfaces/cloudide_plugin_.Plugin.md)<`T`\> \| `undefined`

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

[`Plugin`](../interfaces/cloudide_plugin_.Plugin.md)<`T`\> \| `undefined`

An plug-in or `undefined`.

#### Defined in

[index.d.ts:204](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L204)

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
