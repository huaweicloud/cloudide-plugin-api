[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Extension

# Interface: Extension<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).Extension

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
- [packageJSON](codearts_plugin_.Extension.md#packagejson)

### Methods

- [activate](codearts_plugin_.Extension.md#activate)

## Properties

### exports

• `Readonly` **exports**: `T`

#### Defined in

[index.d.ts:6779](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6779)

___

### extensionKind

• **extensionKind**: [`ExtensionKind`](../enums/codearts_plugin_.ExtensionKind.md)

#### Defined in

[index.d.ts:6773](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6773)

___

### extensionPath

• `Readonly` **extensionPath**: `string`

#### Defined in

[index.d.ts:6754](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6754)

___

### extensionUri

• `Readonly` **extensionUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:6748](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6748)

___

### id

• `Readonly` **id**: `string`

#### Defined in

[index.d.ts:6743](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6743)

___

### isActive

• `Readonly` **isActive**: `boolean`

#### Defined in

[index.d.ts:6759](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6759)

___

### packageJSON

• `Readonly` **packageJSON**: `any`

#### Defined in

[index.d.ts:6764](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6764)

## Methods

### activate

▸ **activate**(): [`Thenable`](Thenable.md)<`T`\>

#### Returns

[`Thenable`](Thenable.md)<`T`\>

#### Defined in

[index.d.ts:6786](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L6786)
