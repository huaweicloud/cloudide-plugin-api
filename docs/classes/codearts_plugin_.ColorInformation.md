[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ColorInformation

# Class: ColorInformation

["@codearts/plugin"](../modules/_codearts_plugin_.md).ColorInformation

Represents a color range from a document.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.ColorInformation.md#constructor)

### Properties

- [color](codearts_plugin_.ColorInformation.md#color)
- [range](codearts_plugin_.ColorInformation.md#range)

## Constructors

### constructor

• **new ColorInformation**(`range`, `color`)

Creates a new color range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) | The range the color appears in. Must not be empty. |
| `color` | [`Color`](codearts_plugin_.Color.md) | The value of the color. |

#### Defined in

[index.d.ts:4826](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L4826)

## Properties

### color

• **color**: [`Color`](codearts_plugin_.Color.md)

The actual color value for this color range.

#### Defined in

[index.d.ts:4818](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L4818)

___

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

The range in the document where this color appears.

#### Defined in

[index.d.ts:4813](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L4813)
