**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](_index_d_.md) / ["plugin"](_index_d_._plugin_.md) / extensions

# Namespace: extensions

Namespace for dealing with installed extensions. Extensions are represented
by an [extension](#Extension)-interface which enables reflection on them.

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
to `package.json`, and use the [getExtension](#extensions.getExtension)-function
and the [exports](#Extension.exports)-property, like below:

```javascript
let mathExt = extensions.getExtension('genius.math');
let importedApi = mathExt.exports;

console.log(importedApi.mul(42, 1));
```

## Index

### Variables

* [all](_index_d_._plugin_.extensions.md#all)
* [onDidChange](_index_d_._plugin_.extensions.md#ondidchange)

### Functions

* [getExtension](_index_d_._plugin_.extensions.md#getextension)

## Variables

### all

• `Const` **all**: ReadonlyArray\<[Extension](../interfaces/_index_d_._plugin_.extension.md)\<any>>

*Defined in [index.d.ts:10702](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10702)*

All extensions currently known to the system.

___

### onDidChange

• `Const` **onDidChange**: [Event](../interfaces/_index_d_._plugin_.event.md)\<void>

*Defined in [index.d.ts:10708](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10708)*

An event which fires when `extensions.all` changes. This can happen when extensions are
installed, uninstalled, enabled or disabled.

## Functions

### getExtension

▸ **getExtension**(`extensionId`: string): [Extension](../interfaces/_index_d_._plugin_.extension.md)\<any> \| undefined

*Defined in [index.d.ts:10689](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10689)*

Get an extension by its full identifier in the form of: `publisher.name`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`extensionId` | string | An extension identifier. |

**Returns:** [Extension](../interfaces/_index_d_._plugin_.extension.md)\<any> \| undefined

An extension or `undefined`.

▸ **getExtension**\<T>(`extensionId`: string): [Extension](../interfaces/_index_d_._plugin_.extension.md)\<T> \| undefined

*Defined in [index.d.ts:10697](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10697)*

Get an extension by its full identifier in the form of: `publisher.name`.

#### Type parameters:

Name |
------ |
`T` |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`extensionId` | string | An extension identifier. |

**Returns:** [Extension](../interfaces/_index_d_._plugin_.extension.md)\<T> \| undefined

An extension or `undefined`.
