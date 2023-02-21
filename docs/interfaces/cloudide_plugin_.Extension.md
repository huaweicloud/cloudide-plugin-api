[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Extension

# Interface: Extension<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Extension

Compatible with vscode
Represents an extension.

To get an instance of an `Extension` use [getExtension](#extensions.getExtension).

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Properties

- [exports](cloudide_plugin_.Extension.md#exports)
- [extensionKind](cloudide_plugin_.Extension.md#extensionkind)
- [extensionPath](cloudide_plugin_.Extension.md#extensionpath)
- [extensionUri](cloudide_plugin_.Extension.md#extensionuri)
- [id](cloudide_plugin_.Extension.md#id)
- [isActive](cloudide_plugin_.Extension.md#isactive)
- [packageJSON](cloudide_plugin_.Extension.md#packagejson)

### Methods

- [activate](cloudide_plugin_.Extension.md#activate)

## Properties

### exports

• `Readonly` **exports**: `T`

The public API exported by this extension. It is an invalid action
to access this field before this extension has been activated.

#### Defined in

[index.d.ts:151](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L151)

___

### extensionKind

• **extensionKind**: `ExtensionKind`

The extension kind describes if an extension runs where the UI runs
or if an extension runs where the remote extension host runs. The extension kind
is defined in the `package.json`-file of extensions but can also be refined
via the `remote.extensionKind`-setting. When no remote extension host exists,
the value is [`ExtensionKind.UI`](#ExtensionKind.UI).

#### Defined in

[index.d.ts:145](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L145)

___

### extensionPath

• `Readonly` **extensionPath**: `string`

The absolute file path of the directory containing this extension. Shorthand
notation for [Extension.extensionUri.fsPath](#Extension.extensionUri) (independent of the uri scheme).

#### Defined in

[index.d.ts:126](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L126)

___

### extensionUri

• `Readonly` **extensionUri**: [`Uri`](../classes/cloudide_plugin_.Uri.md)

The uri of the directory containing the extension.

#### Defined in

[index.d.ts:120](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L120)

___

### id

• `Readonly` **id**: `string`

The canonical extension identifier in the form of: `publisher.name`.

#### Defined in

[index.d.ts:115](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L115)

___

### isActive

• `Readonly` **isActive**: `boolean`

`true` if the extension has been activated.

#### Defined in

[index.d.ts:131](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L131)

___

### packageJSON

• `Readonly` **packageJSON**: `any`

The parsed contents of the extension's package.json.

#### Defined in

[index.d.ts:136](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L136)

## Methods

### activate

▸ **activate**(): [`Thenable`](Thenable.md)<`T`\>

Activates this extension and returns its public API.

#### Returns

[`Thenable`](Thenable.md)<`T`\>

A promise that will resolve when this extension has been activated.

#### Defined in

[index.d.ts:158](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L158)
