[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / LinkedEditingRanges

# Class: LinkedEditingRanges

["@codearts/plugin"](../modules/_codearts_plugin_.md).LinkedEditingRanges

Represents a list of ranges that can be edited together along with a word pattern to describe valid range contents.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.LinkedEditingRanges.md#constructor)

### Properties

- [ranges](codearts_plugin_.LinkedEditingRanges.md#ranges)
- [wordPattern](codearts_plugin_.LinkedEditingRanges.md#wordpattern)

## Constructors

### constructor

• **new LinkedEditingRanges**(`ranges`, `wordPattern?`)

Create a new linked editing ranges object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ranges` | [`Range`](codearts_plugin_.Range.md)[] | A list of ranges that can be edited together |
| `wordPattern?` | `RegExp` | An optional word pattern that describes valid contents for the given ranges |

#### Defined in

[index.d.ts:5456](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5456)

## Properties

### ranges

• `Readonly` **ranges**: [`Range`](codearts_plugin_.Range.md)[]

A list of ranges that can be edited together. The ranges must have
identical length and text content. The ranges cannot overlap.

#### Defined in

[index.d.ts:5462](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5462)

___

### wordPattern

• `Readonly` **wordPattern**: `undefined` \| `RegExp`

An optional word pattern that describes valid contents for the given ranges.
If no pattern is provided, the language configuration's word pattern will be used.

#### Defined in

[index.d.ts:5468](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5468)
