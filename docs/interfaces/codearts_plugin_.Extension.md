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

[index.d.ts:6901](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6901)

___

### extensionKind

• **extensionKind**: [`ExtensionKind`](../enums/codearts_plugin_.ExtensionKind.md)

The extension kind describes if an extension runs where the UI runs
or if an extension runs where the remote extension host runs. The extension kind
is defined in the `package.json`-file of extensions but can also be refined
via the `remote.extensionKind`-setting. When no remote extension host exists,
the value is [`UI`](../enums/codearts_plugin_.ExtensionKind.md#ui).

#### Defined in

[index.d.ts:6895](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6895)

___

### extensionPath

• `Readonly` **extensionPath**: `string`

The absolute file path of the directory containing this extension. Shorthand
notation for [Extension.extensionUri.fsPath](codearts_plugin_.Extension.md#extensionuri) (independent of the uri scheme).

#### Defined in

[index.d.ts:6876](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6876)

___

### extensionUri

• `Readonly` **extensionUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The uri of the directory containing the extension.

#### Defined in

[index.d.ts:6870](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6870)

___

### id

• `Readonly` **id**: `string`

The canonical extension identifier in the form of: `publisher.name`.

#### Defined in

[index.d.ts:6865](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6865)

___

### isActive

• `Readonly` **isActive**: `boolean`

`true` if the extension has been activated.

#### Defined in

[index.d.ts:6881](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6881)

___

### onDidActivate

• `Readonly` **onDidActivate**: [`Event`](codearts_plugin_.Event.md)<`void`\>

An event which fires when this extension has been activated.

#### Defined in

[index.d.ts:6913](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6913)

___

### packageJSON

• `Readonly` **packageJSON**: `any`

The parsed contents of the extension's package.json.

#### Defined in

[index.d.ts:6886](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6886)

## Methods

### activate

▸ **activate**(): [`Thenable`](Thenable.md)<`T`\>

Activates this extension and returns its public API.

#### Returns

[`Thenable`](Thenable.md)<`T`\>

A promise that will resolve when this extension has been activated.

#### Defined in

[index.d.ts:6908](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6908)
