**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / LinkedEditingRanges

# Class: LinkedEditingRanges

Represents a list of ranges that can be edited together along with a word pattern to describe valid range contents.

## Hierarchy

* **LinkedEditingRanges**

## Index

### Constructors

* [constructor](_index_d_._plugin_.linkededitingranges.md#constructor)

### Properties

* [ranges](_index_d_._plugin_.linkededitingranges.md#ranges)
* [wordPattern](_index_d_._plugin_.linkededitingranges.md#wordpattern)

## Constructors

### constructor

\+ **new LinkedEditingRanges**(`ranges`: [Range](_index_d_._plugin_.range.md)[], `wordPattern?`: RegExp): [LinkedEditingRanges](_index_d_._plugin_.linkededitingranges.md)

*Defined in [index.d.ts:4679](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4679)*

Create a new linked editing ranges object.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`ranges` | [Range](_index_d_._plugin_.range.md)[] | A list of ranges that can be edited together |
`wordPattern?` | RegExp | An optional word pattern that describes valid contents for the given ranges  |

**Returns:** [LinkedEditingRanges](_index_d_._plugin_.linkededitingranges.md)

## Properties

### ranges

• `Readonly` **ranges**: [Range](_index_d_._plugin_.range.md)[]

*Defined in [index.d.ts:4692](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4692)*

A list of ranges that can be edited together. The ranges must have
identical length and text content. The ranges cannot overlap.

___

### wordPattern

• `Optional` `Readonly` **wordPattern**: RegExp

*Defined in [index.d.ts:4698](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4698)*

An optional word pattern that describes valid contents for the given ranges.
If no pattern is provided, the language configuration's word pattern will be used.
