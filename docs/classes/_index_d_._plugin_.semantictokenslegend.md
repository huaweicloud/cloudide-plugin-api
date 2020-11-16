**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SemanticTokensLegend

# Class: SemanticTokensLegend

A semantic tokens legend contains the needed information to decipher
the integer encoded representation of semantic tokens.

## Hierarchy

* **SemanticTokensLegend**

## Index

### Constructors

* [constructor](_index_d_._plugin_.semantictokenslegend.md#constructor)

### Properties

* [tokenModifiers](_index_d_._plugin_.semantictokenslegend.md#tokenmodifiers)
* [tokenTypes](_index_d_._plugin_.semantictokenslegend.md#tokentypes)

## Constructors

### constructor

\+ **new SemanticTokensLegend**(`tokenTypes`: string[], `tokenModifiers?`: string[]): [SemanticTokensLegend](_index_d_._plugin_.semantictokenslegend.md)

*Defined in [index.d.ts:3195](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3195)*

#### Parameters:

Name | Type |
------ | ------ |
`tokenTypes` | string[] |
`tokenModifiers?` | string[] |

**Returns:** [SemanticTokensLegend](_index_d_._plugin_.semantictokenslegend.md)

## Properties

### tokenModifiers

• `Readonly` **tokenModifiers**: string[]

*Defined in [index.d.ts:3195](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3195)*

The possible token modifiers.

___

### tokenTypes

• `Readonly` **tokenTypes**: string[]

*Defined in [index.d.ts:3191](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3191)*

The possible token types.
