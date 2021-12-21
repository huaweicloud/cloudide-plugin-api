**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Extension

# Interface: Extension\<T, T>

Compatible with vscode
Represents an extension.
Represents an extension.

To get an instance of an `Extension` use [getExtension](#extensions.getExtension).

To get an instance of an `Extension` use [getExtension](#extensions.getExtension).

## Type parameters

Name |
------ |
`T` |
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

*Defined in [index.d.ts:121](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L121)*

*Defined in [index.d.ts:5870](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5870)*

The public API exported by this extension. It is an invalid action
to access this field before this extension has been activated.
The public API exported by this extension. It is an invalid action
to access this field before this extension has been activated.

___

### extensionKind

•  **extensionKind**: [ExtensionKind](../enums/_index_d_._plugin_.extensionkind.md)

*Defined in [index.d.ts:115](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L115)*

*Defined in [index.d.ts:5864](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5864)*

The extension kind describes if an extension runs where the UI runs
or if an extension runs where the remote extension host runs. The extension kind
is defined in the `package.json`-file of extensions but can also be refined
via the `remote.extensionKind`-setting. When no remote extension host exists,
the value is [`ExtensionKind.UI`](#ExtensionKind.UI).
The extension kind describes if an extension runs where the UI runs
or if an extension runs where the remote extension host runs. The extension kind
is defined in the `package.json`-file of extensions but can also be refined
via the `remote.extensionKind`-setting. When no remote extension host exists,
the value is [`ExtensionKind.UI`](#ExtensionKind.UI).

___

### extensionPath

• `Readonly` **extensionPath**: string

*Defined in [index.d.ts:96](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L96)*

*Defined in [index.d.ts:5845](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5845)*

The absolute file path of the directory containing this extension. Shorthand
notation for [Extension.extensionUri.fsPath](#Extension.extensionUri) (independent of the uri scheme).
The absolute file path of the directory containing this extension. Shorthand
notation for [Extension.extensionUri.fsPath](#Extension.extensionUri) (independent of the uri scheme).

___

### extensionUri

• `Readonly` **extensionUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:90](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L90)*

*Defined in [index.d.ts:5839](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5839)*

The uri of the directory containing the extension.
The uri of the directory containing the extension.

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:85](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L85)*

*Defined in [index.d.ts:5834](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5834)*

The canonical extension identifier in the form of: `publisher.name`.
The canonical extension identifier in the form of: `publisher.name`.

___

### isActive

• `Readonly` **isActive**: boolean

*Defined in [index.d.ts:101](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L101)*

*Defined in [index.d.ts:5850](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5850)*

`true` if the extension has been activated.
`true` if the extension has been activated.

___

### packageJSON

• `Readonly` **packageJSON**: any

*Defined in [index.d.ts:106](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L106)*

*Defined in [index.d.ts:5855](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5855)*

The parsed contents of the extension's package.json.
The parsed contents of the extension's package.json.

## Methods

### activate

▸ **activate**(): [Thenable](_index_d_.thenable.md)\<T>

*Defined in [index.d.ts:128](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L128)*

Activates this extension and returns its public API.

**Returns:** [Thenable](_index_d_.thenable.md)\<T>

A promise that will resolve when this extension has been activated.

▸ **activate**(): [Thenable](_index_d_.thenable.md)\<T>

*Defined in [index.d.ts:5877](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5877)*

Activates this extension and returns its public API.

**Returns:** [Thenable](_index_d_.thenable.md)\<T>

A promise that will resolve when this extension has been activated.
