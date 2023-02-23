[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SemanticTokensEdits

# Class: SemanticTokensEdits

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SemanticTokensEdits

Represents edits to semantic tokens.

**`See`**

[provideDocumentSemanticTokensEdits](#DocumentSemanticTokensProvider.provideDocumentSemanticTokensEdits) for an explanation of the format.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.SemanticTokensEdits.md#constructor)

### Properties

- [edits](cloudide_plugin_.SemanticTokensEdits.md#edits)
- [resultId](cloudide_plugin_.SemanticTokensEdits.md#resultid)

## Constructors

### constructor

• **new SemanticTokensEdits**(`edits`, `resultId?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `edits` | [`SemanticTokensEdit`](cloudide_plugin_.SemanticTokensEdit.md)[] |
| `resultId?` | `string` |

#### Defined in

[index.d.ts:8623](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8623)

## Properties

### edits

• `Readonly` **edits**: [`SemanticTokensEdit`](cloudide_plugin_.SemanticTokensEdit.md)[]

The edits to the tokens data.
All edits refer to the initial data state.

#### Defined in

[index.d.ts:8621](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8621)

___

### resultId

• `Optional` `Readonly` **resultId**: `string`

The result id of the tokens.

This is the id that will be passed to `DocumentSemanticTokensProvider.provideDocumentSemanticTokensEdits` (if implemented).

#### Defined in

[index.d.ts:8616](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8616)
