[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CodeActionKind

# Class: CodeActionKind

["@codearts/plugin"](../modules/_codearts_plugin_.md).CodeActionKind

## Table of contents

### Constructors

- [constructor](codearts_plugin_.CodeActionKind.md#constructor)

### Properties

- [value](codearts_plugin_.CodeActionKind.md#value)
- [Empty](codearts_plugin_.CodeActionKind.md#empty)
- [QuickFix](codearts_plugin_.CodeActionKind.md#quickfix)
- [Refactor](codearts_plugin_.CodeActionKind.md#refactor)
- [RefactorExtract](codearts_plugin_.CodeActionKind.md#refactorextract)
- [RefactorInline](codearts_plugin_.CodeActionKind.md#refactorinline)
- [RefactorRewrite](codearts_plugin_.CodeActionKind.md#refactorrewrite)
- [Source](codearts_plugin_.CodeActionKind.md#source)
- [SourceFixAll](codearts_plugin_.CodeActionKind.md#sourcefixall)
- [SourceOrganizeImports](codearts_plugin_.CodeActionKind.md#sourceorganizeimports)

### Methods

- [append](codearts_plugin_.CodeActionKind.md#append)
- [contains](codearts_plugin_.CodeActionKind.md#contains)
- [intersects](codearts_plugin_.CodeActionKind.md#intersects)

## Constructors

### constructor

• `Private` **new CodeActionKind**(`value`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Defined in

[index.d.ts:2323](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2323)

## Properties

### value

• `Readonly` **value**: `string`

#### Defined in

[index.d.ts:2328](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2328)

___

### Empty

▪ `Static` `Readonly` **Empty**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

#### Defined in

[index.d.ts:2246](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2246)

___

### QuickFix

▪ `Static` `Readonly` **QuickFix**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

#### Defined in

[index.d.ts:2253](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2253)

___

### Refactor

▪ `Static` `Readonly` **Refactor**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

#### Defined in

[index.d.ts:2260](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2260)

___

### RefactorExtract

▪ `Static` `Readonly` **RefactorExtract**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

#### Defined in

[index.d.ts:2273](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2273)

___

### RefactorInline

▪ `Static` `Readonly` **RefactorInline**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

#### Defined in

[index.d.ts:2285](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2285)

___

### RefactorRewrite

▪ `Static` `Readonly` **RefactorRewrite**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

#### Defined in

[index.d.ts:2299](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2299)

___

### Source

▪ `Static` `Readonly` **Source**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

#### Defined in

[index.d.ts:2308](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2308)

___

### SourceFixAll

▪ `Static` `Readonly` **SourceFixAll**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

#### Defined in

[index.d.ts:2321](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2321)

___

### SourceOrganizeImports

▪ `Static` `Readonly` **SourceOrganizeImports**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

#### Defined in

[index.d.ts:2313](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2313)

## Methods

### append

▸ **append**(`parts`): [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `parts` | `string` |

#### Returns

[`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

#### Defined in

[index.d.ts:2335](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2335)

___

### contains

▸ **contains**(`other`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`CodeActionKind`](codearts_plugin_.CodeActionKind.md) |  |

#### Returns

`boolean`

#### Defined in

[index.d.ts:2355](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2355)

___

### intersects

▸ **intersects**(`other`): `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`CodeActionKind`](codearts_plugin_.CodeActionKind.md) |  |

#### Returns

`boolean`

#### Defined in

[index.d.ts:2345](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2345)
