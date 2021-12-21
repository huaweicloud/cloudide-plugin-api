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

*Defined in [index.d.ts:3518](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3518)*

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

*Defined in [index.d.ts:3518](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3518)*

The elements to insert.

___

### deleteCount

• `Readonly` **deleteCount**: number

*Defined in [index.d.ts:3514](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3514)*

The count of elements to remove.

___

### start

• `Readonly` **start**: number

*Defined in [index.d.ts:3510](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3510)*

The start offset of the edit.
