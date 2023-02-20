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

*Defined in [index.d.ts:124](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L124)*

*Defined in [index.d.ts:5873](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5873)*

The public API exported by this extension. It is an invalid action
to access this field before this extension has been activated.
The public API exported by this extension. It is an invalid action
to access this field before this extension has been activated.

___

### extensionKind

•  **extensionKind**: [ExtensionKind](../enums/_index_d_._plugin_.extensionkind.md)

*Defined in [index.d.ts:118](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L118)*

*Defined in [index.d.ts:5867](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5867)*

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

*Defined in [index.d.ts:99](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L99)*

*Defined in [index.d.ts:5848](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5848)*

The absolute file path of the directory containing this extension. Shorthand
notation for [Extension.extensionUri.fsPath](#Extension.extensionUri) (independent of the uri scheme).
The absolute file path of the directory containing this extension. Shorthand
notation for [Extension.extensionUri.fsPath](#Extension.extensionUri) (independent of the uri scheme).

___

### extensionUri

• `Readonly` **extensionUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:93](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L93)*

*Defined in [index.d.ts:5842](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5842)*

The uri of the directory containing the extension.
The uri of the directory containing the extension.

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:88](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L88)*

*Defined in [index.d.ts:5837](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5837)*

The canonical extension identifier in the form of: `publisher.name`.
The canonical extension identifier in the form of: `publisher.name`.

___

### isActive

• `Readonly` **isActive**: boolean

*Defined in [index.d.ts:104](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L104)*

*Defined in [index.d.ts:5853](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5853)*

`true` if the extension has been activated.
`true` if the extension has been activated.

___

### packageJSON

• `Readonly` **packageJSON**: any

*Defined in [index.d.ts:109](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L109)*

*Defined in [index.d.ts:5858](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5858)*

The parsed contents of the extension's package.json.
The parsed contents of the extension's package.json.

## Methods

### activate

▸ **activate**(): [Thenable](_index_d_.thenable.md)\<T>

*Defined in [index.d.ts:131](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L131)*

Activates this extension and returns its public API.

**Returns:** [Thenable](_index_d_.thenable.md)\<T>

A promise that will resolve when this extension has been activated.

▸ **activate**(): [Thenable](_index_d_.thenable.md)\<T>

*Defined in [index.d.ts:5880](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5880)*

Activates this extension and returns its public API.

**Returns:** [Thenable](_index_d_.thenable.md)\<T>

A promise that will resolve when this extension has been activated.
