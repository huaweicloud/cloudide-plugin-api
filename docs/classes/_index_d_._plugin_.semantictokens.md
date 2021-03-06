**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SemanticTokens

# Class: SemanticTokens

Represents semantic tokens, either in a range or in an entire document.

**`see`** [provideDocumentSemanticTokens](#DocumentSemanticTokensProvider.provideDocumentSemanticTokens) for an explanation of the format.

**`see`** [SemanticTokensBuilder](#SemanticTokensBuilder) for a helper to create an instance.

## Hierarchy

* **SemanticTokens**

## Index

### Constructors

* [constructor](_index_d_._plugin_.semantictokens.md#constructor)

### Properties

* [data](_index_d_._plugin_.semantictokens.md#data)
* [resultId](_index_d_._plugin_.semantictokens.md#resultid)

## Constructors

### constructor

\+ **new SemanticTokens**(`data`: Uint32Array, `resultId?`: string): [SemanticTokens](_index_d_._plugin_.semantictokens.md)

*Defined in [index.d.ts:3250](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3250)*

#### Parameters:

Name | Type |
------ | ------ |
`data` | Uint32Array |
`resultId?` | string |

**Returns:** [SemanticTokens](_index_d_._plugin_.semantictokens.md)

## Properties

### data

• `Readonly` **data**: Uint32Array

*Defined in [index.d.ts:3250](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3250)*

The actual tokens data.

**`see`** [provideDocumentSemanticTokens](#DocumentSemanticTokensProvider.provideDocumentSemanticTokens) for an explanation of the format.

___

### resultId

• `Optional` `Readonly` **resultId**: string

*Defined in [index.d.ts:3245](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3245)*

The result id of the tokens.

This is the id that will be passed to `DocumentSemanticTokensProvider.provideDocumentSemanticTokensEdits` (if implemented).
