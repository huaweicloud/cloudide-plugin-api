**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SemanticTokensEdits

# Class: SemanticTokensEdits

Represents edits to semantic tokens.

**`see`** [provideDocumentSemanticTokensEdits](#DocumentSemanticTokensProvider.provideDocumentSemanticTokensEdits) for an explanation of the format.

## Hierarchy

* **SemanticTokensEdits**

## Index

### Constructors

* [constructor](_index_d_._plugin_.semantictokensedits.md#constructor)

### Properties

* [edits](_index_d_._plugin_.semantictokensedits.md#edits)
* [resultId](_index_d_._plugin_.semantictokensedits.md#resultid)

## Constructors

### constructor

\+ **new SemanticTokensEdits**(`edits`: [SemanticTokensEdit](_index_d_._plugin_.semantictokensedit.md)[], `resultId?`: string): [SemanticTokensEdits](_index_d_._plugin_.semantictokensedits.md)

*Defined in [index.d.ts:3500](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3500)*

#### Parameters:

Name | Type |
------ | ------ |
`edits` | [SemanticTokensEdit](_index_d_._plugin_.semantictokensedit.md)[] |
`resultId?` | string |

**Returns:** [SemanticTokensEdits](_index_d_._plugin_.semantictokensedits.md)

## Properties

### edits

• `Readonly` **edits**: [SemanticTokensEdit](_index_d_._plugin_.semantictokensedit.md)[]

*Defined in [index.d.ts:3500](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3500)*

The edits to the tokens data.
All edits refer to the initial data state.

___

### resultId

• `Optional` `Readonly` **resultId**: string

*Defined in [index.d.ts:3495](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L3495)*

The result id of the tokens.

This is the id that will be passed to `DocumentSemanticTokensProvider.provideDocumentSemanticTokensEdits` (if implemented).
