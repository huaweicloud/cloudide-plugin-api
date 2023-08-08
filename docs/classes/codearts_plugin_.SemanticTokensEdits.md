[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SemanticTokensEdits

# Class: SemanticTokensEdits

["@codearts/plugin"](../modules/_codearts_plugin_.md).SemanticTokensEdits

Represents edits to semantic tokens.

**`See`**

[provideDocumentSemanticTokensEdits](../interfaces/codearts_plugin_.DocumentSemanticTokensProvider.md#providedocumentsemantictokensedits) for an explanation of the format.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.SemanticTokensEdits.md#constructor)

### Properties

- [edits](codearts_plugin_.SemanticTokensEdits.md#edits)
- [resultId](codearts_plugin_.SemanticTokensEdits.md#resultid)

## Constructors

### constructor

• **new SemanticTokensEdits**(`edits`, `resultId?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `edits` | [`SemanticTokensEdit`](codearts_plugin_.SemanticTokensEdit.md)[] |
| `resultId?` | `string` |

#### Defined in

[index.d.ts:3806](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3806)

## Properties

### edits

• `Readonly` **edits**: [`SemanticTokensEdit`](codearts_plugin_.SemanticTokensEdit.md)[]

The edits to the tokens data.
All edits refer to the initial data state.

#### Defined in

[index.d.ts:3804](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3804)

___

### resultId

• `Readonly` **resultId**: `undefined` \| `string`

The result id of the tokens.

This is the id that will be passed to `DocumentSemanticTokensProvider.provideDocumentSemanticTokensEdits` (if implemented).

#### Defined in

[index.d.ts:3799](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3799)
