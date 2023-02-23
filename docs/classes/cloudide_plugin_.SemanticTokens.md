[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SemanticTokens

# Class: SemanticTokens

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SemanticTokens

Represents semantic tokens, either in a range or in an entire document.

**`See`**

 - [provideDocumentSemanticTokens](#DocumentSemanticTokensProvider.provideDocumentSemanticTokens) for an explanation of the format.
 - [SemanticTokensBuilder](#SemanticTokensBuilder) for a helper to create an instance.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.SemanticTokens.md#constructor)

### Properties

- [data](cloudide_plugin_.SemanticTokens.md#data)
- [resultId](cloudide_plugin_.SemanticTokens.md#resultid)

## Constructors

### constructor

• **new SemanticTokens**(`data`, `resultId?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | `Uint32Array` |
| `resultId?` | `string` |

#### Defined in

[index.d.ts:8603](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8603)

## Properties

### data

• `Readonly` **data**: `Uint32Array`

The actual tokens data.

**`See`**

[provideDocumentSemanticTokens](#DocumentSemanticTokensProvider.provideDocumentSemanticTokens) for an explanation of the format.

#### Defined in

[index.d.ts:8601](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8601)

___

### resultId

• `Optional` `Readonly` **resultId**: `string`

The result id of the tokens.

This is the id that will be passed to `DocumentSemanticTokensProvider.provideDocumentSemanticTokensEdits` (if implemented).

#### Defined in

[index.d.ts:8596](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8596)
