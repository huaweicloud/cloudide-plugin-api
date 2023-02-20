**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SemanticTokensEdit

# Class: SemanticTokensEdit

Represents an edit to semantic tokens.

**`see`** [provideDocumentSemanticTokensEdits](#DocumentSemanticTokensProvider.provideDocumentSemanticTokensEdits) for an explanation of the format.

## Hierarchy

* **SemanticTokensEdit**

## Index

### Constructors

* [constructor](_index_d_._plugin_.semantictokensedit.md#constructor)

### Properties

* [data](_index_d_._plugin_.semantictokensedit.md#data)
* [deleteCount](_index_d_._plugin_.semantictokensedit.md#deletecount)
* [start](_index_d_._plugin_.semantictokensedit.md#start)

## Constructors

### constructor

\+ **new SemanticTokensEdit**(`start`: number, `deleteCount`: number, `data?`: Uint32Array): [SemanticTokensEdit](_index_d_._plugin_.semantictokensedit.md)

*Defined in [index.d.ts:3521](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L3521)*

#### Parameters:

Name | Type |
------ | ------ |
`start` | number |
`deleteCount` | number |
`data?` | Uint32Array |

**Returns:** [SemanticTokensEdit](_index_d_._plugin_.semantictokensedit.md)

## Properties

### data

• `Optional` `Readonly` **data**: Uint32Array

*Defined in [index.d.ts:3521](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L3521)*

The elements to insert.

___

### deleteCount

• `Readonly` **deleteCount**: number

*Defined in [index.d.ts:3517](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L3517)*

The count of elements to remove.

___

### start

• `Readonly` **start**: number

*Defined in [index.d.ts:3513](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L3513)*

The start offset of the edit.
