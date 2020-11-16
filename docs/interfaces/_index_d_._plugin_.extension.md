**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Extension

# Interface: Extension\<T>

Represents an extension.

To get an instance of an `Extension` use [getExtension](#extensions.getExtension).

## Type parameters

Name |
------ |
`T` |

## Hierarchy

* **Extension**

## Index

### Properties

* [exports](_index_d_._plugin_.extension.md#exports)
* [extensionKind](_index_d_._plugin_.extension.md#extensionkind)
* [extensionPath](_index_d_._plugin_.extension.md#extensionpath)
* [extensionUri](_index_d_._plugin_.extension.md#extensionuri)
* [id](_index_d_._plugin_.extension.md#id)
* [isActive](_index_d_._plugin_.extension.md#isactive)
* [packageJSON](_index_d_._plugin_.extension.md#packagejson)

### Methods

* [activate](_index_d_._plugin_.extension.md#activate)

## Properties

### exports

• `Readonly` **exports**: T

*Defined in [index.d.ts:5415](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5415)*

The public API exported by this extension. It is an invalid action
to access this field before this extension has been activated.

___

### extensionKind

•  **extensionKind**: [ExtensionKind](../enums/_index_d_._plugin_.extensionkind.md)

*Defined in [index.d.ts:5409](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5409)*

The extension kind describes if an extension runs where the UI runs
or if an extension runs where the remote extension host runs. The extension kind
is defined in the `package.json`-file of extensions but can also be refined
via the `remote.extensionKind`-setting. When no remote extension host exists,
the value is [`ExtensionKind.UI`](#ExtensionKind.UI).

___

### extensionPath

• `Readonly` **extensionPath**: string

*Defined in [index.d.ts:5390](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5390)*

The absolute file path of the directory containing this extension. Shorthand
notation for [Extension.extensionUri.fsPath](#Extension.extensionUri) (independent of the uri scheme).

___

### extensionUri

• `Readonly` **extensionUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:5384](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5384)*

The uri of the directory containing the extension.

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:5379](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5379)*

The canonical extension identifier in the form of: `publisher.name`.

___

### isActive

• `Readonly` **isActive**: boolean

*Defined in [index.d.ts:5395](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5395)*

`true` if the extension has been activated.

___

### packageJSON

• `Readonly` **packageJSON**: any

*Defined in [index.d.ts:5400](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5400)*

The parsed contents of the extension's package.json.

## Methods

### activate

▸ **activate**(): [Thenable](_index_d_.thenable.md)\<T>

*Defined in [index.d.ts:5422](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5422)*

Activates this extension and returns its public API.

**Returns:** [Thenable](_index_d_.thenable.md)\<T>

A promise that will resolve when this extension has been activated.
