[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SemanticTokensEdit

# Class: SemanticTokensEdit

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SemanticTokensEdit

Represents an edit to semantic tokens.

**`See`**

[provideDocumentSemanticTokensEdits](#DocumentSemanticTokensProvider.provideDocumentSemanticTokensEdits) for an explanation of the format.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.SemanticTokensEdit.md#constructor)

### Properties

- [data](cloudide_plugin_.SemanticTokensEdit.md#data)
- [deleteCount](cloudide_plugin_.SemanticTokensEdit.md#deletecount)
- [start](cloudide_plugin_.SemanticTokensEdit.md#start)

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

[index.d.ts:8644](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8644)

## Properties

### data

• `Optional` `Readonly` **data**: `Uint32Array`

The elements to insert.

#### Defined in

[index.d.ts:8642](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8642)

___

### deleteCount

• `Readonly` **deleteCount**: `number`

The count of elements to remove.

#### Defined in

[index.d.ts:8638](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8638)

___

### start

• `Readonly` **start**: `number`

The start offset of the edit.

#### Defined in

[index.d.ts:8634](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8634)
