[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ColorInformation

# Class: ColorInformation

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ColorInformation

Represents a color range from a document.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.ColorInformation.md#constructor)

### Properties

- [color](cloudide_plugin_.ColorInformation.md#color)
- [range](cloudide_plugin_.ColorInformation.md#range)

## Constructors

### constructor

• **new ColorInformation**(`range`, `color`)

Creates a new color range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](cloudide_plugin_.Range.md) | The range the color appears in. Must not be empty. |
| `color` | [`Color`](cloudide_plugin_.Color.md) | The value of the color. |

#### Defined in

[index.d.ts:7162](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7162)

## Properties

### color

• **color**: [`Color`](cloudide_plugin_.Color.md)

The actual color value for this color range.

#### Defined in

[index.d.ts:7154](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7154)

___

### range

• **range**: [`Range`](cloudide_plugin_.Range.md)

The range in the document where this color appears.

#### Defined in

[index.d.ts:7149](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7149)
