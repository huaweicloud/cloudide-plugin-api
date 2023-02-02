[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SemanticTokensEdit

# Class: SemanticTokensEdit

["@codearts/plugin"](../modules/_codearts_plugin_.md).SemanticTokensEdit

Represents an edit to semantic tokens.

**`See`**

[provideDocumentSemanticTokensEdits](../interfaces/codearts_plugin_.DocumentSemanticTokensProvider.md#providedocumentsemantictokensedits) for an explanation of the format.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.SemanticTokensEdit.md#constructor)

### Properties

- [data](codearts_plugin_.SemanticTokensEdit.md#data)
- [deleteCount](codearts_plugin_.SemanticTokensEdit.md#deletecount)
- [start](codearts_plugin_.SemanticTokensEdit.md#start)

## Constructors

### constructor

• **new SemanticTokensEdit**(`start`, `deleteCount`, `data?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `start` | `number` |
| `deleteCount` | `number` |
| `data?` | `Uint32Array` |

#### Defined in

[index.d.ts:3789](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L3789)

## Properties

### data

• `Readonly` **data**: `undefined` \| `Uint32Array`

The elements to insert.

#### Defined in

[index.d.ts:3787](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L3787)

___

### deleteCount

• `Readonly` **deleteCount**: `number`

The count of elements to remove.

#### Defined in

[index.d.ts:3783](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L3783)

___

### start

• `Readonly` **start**: `number`

The start offset of the edit.

#### Defined in

[index.d.ts:3779](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L3779)
