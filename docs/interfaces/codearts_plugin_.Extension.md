[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Extension

# Interface: Extension<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).Extension

Represents an extension.

To get an instance of an `Extension` use [getExtension](../modules/codearts_plugin_.extensions.md#getextension).

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Properties

- [exports](codearts_plugin_.Extension.md#exports)
- [extensionKind](codearts_plugin_.Extension.md#extensionkind)
- [extensionPath](codearts_plugin_.Extension.md#extensionpath)
- [extensionUri](codearts_plugin_.Extension.md#extensionuri)
- [id](codearts_plugin_.Extension.md#id)
- [isActive](codearts_plugin_.Extension.md#isactive)
- [onDidActivate](codearts_plugin_.Extension.md#ondidactivate)
- [packageJSON](codearts_plugin_.Extension.md#packagejson)

### Methods

- [activate](codearts_plugin_.Extension.md#activate)

## Properties

### exports

• `Readonly` **exports**: `T`

The public API exported by this extension (return value of `activate`).
It is an invalid action to access this field before this extension has been activated.

#### Defined in

[index.d.ts:6872](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6872)

___

### extensionKind

• **extensionKind**: [`ExtensionKind`](../enums/codearts_plugin_.ExtensionKind.md)

The extension kind describes if an extension runs where the UI runs
or if an extension runs where the remote extension host runs. The extension kind
is defined in the `package.json`-file of extensions but can also be refined
via the `remote.extensionKind`-setting. When no remote extension host exists,
the value is [`UI`](../enums/codearts_plugin_.ExtensionKind.md#ui).

#### Defined in

[index.d.ts:6866](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6866)

___

### extensionPath

• `Readonly` **extensionPath**: `string`

The absolute file path of the directory containing this extension. Shorthand
notation for [Extension.extensionUri.fsPath](codearts_plugin_.Extension.md#extensionuri) (independent of the uri scheme).

#### Defined in

[index.d.ts:6847](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6847)

___

### extensionUri

• `Readonly` **extensionUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The uri of the directory containing the extension.

#### Defined in

[index.d.ts:6841](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6841)

___

### id

• `Readonly` **id**: `string`

The canonical extension identifier in the form of: `publisher.name`.

#### Defined in

[index.d.ts:6836](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6836)

___

### isActive

• `Readonly` **isActive**: `boolean`

`true` if the extension has been activated.

#### Defined in

[index.d.ts:6852](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6852)

___

### onDidActivate

• `Readonly` **onDidActivate**: [`Event`](codearts_plugin_.Event.md)<`void`\>

An event which fires when this extension has been activated.

#### Defined in

[index.d.ts:6884](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6884)

___

### packageJSON

• `Readonly` **packageJSON**: `any`

The parsed contents of the extension's package.json.

#### Defined in

[index.d.ts:6857](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6857)

## Methods

### activate

▸ **activate**(): [`Thenable`](Thenable.md)<`T`\>

Activates this extension and returns its public API.

#### Returns

[`Thenable`](Thenable.md)<`T`\>

A promise that will resolve when this extension has been activated.

#### Defined in

[index.d.ts:6879](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6879)
