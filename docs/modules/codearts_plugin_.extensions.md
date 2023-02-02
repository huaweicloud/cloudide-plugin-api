[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / extensions

# Namespace: extensions

["@codearts/plugin"](_codearts_plugin_.md).extensions

Namespace for dealing with installed extensions. Extensions are represented
by an [Extension](../interfaces/codearts_plugin_.Extension.md)-interface which enables reflection on them.

Extension writers can provide APIs to other extensions by returning their API public
surface from the `activate`-call.

```javascript
export function activate(context: vscode.ExtensionContext) {
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
When depending on the API of another extension add an `extensionDependencies`-entry
to `package.json`, and use the [getExtension](codearts_plugin_.extensions.md#getextension)-function
and the [exports](../interfaces/codearts_plugin_.Extension.md#exports)-property, like below:

```javascript
let mathExt = extensions.getExtension('genius.math');
let importedApi = mathExt.exports;

console.log(importedApi.mul(42, 1));
```

## Table of contents

### Variables

- [all](codearts_plugin_.extensions.md#all)

### Functions

- [getExtension](codearts_plugin_.extensions.md#getextension)
- [onDidChange](codearts_plugin_.extensions.md#ondidchange)

## Variables

### all

• `Const` **all**: readonly [`Extension`](../interfaces/codearts_plugin_.Extension.md)<`any`\>[]

All extensions currently known to the system.

#### Defined in

[index.d.ts:15130](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15130)

## Functions

### getExtension

▸ **getExtension**<`T`\>(`extensionId`): [`Extension`](../interfaces/codearts_plugin_.Extension.md)<`T`\> \| `undefined`

Get an extension by its full identifier in the form of: `publisher.name`.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `any` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `extensionId` | `string` | An extension identifier. |

#### Returns

[`Extension`](../interfaces/codearts_plugin_.Extension.md)<`T`\> \| `undefined`

An extension or `undefined`.

#### Defined in

[index.d.ts:15125](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15125)

___

### onDidChange

▸ **onDidChange**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: `void`) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1603)
