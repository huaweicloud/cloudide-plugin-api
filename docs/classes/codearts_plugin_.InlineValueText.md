[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlineValueText

# Class: InlineValueText

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlineValueText

Provide inline value as text.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.InlineValueText.md#constructor)

### Properties

- [range](codearts_plugin_.InlineValueText.md#range)
- [text](codearts_plugin_.InlineValueText.md#text)

## Constructors

### constructor

• **new InlineValueText**(`range`, `text`)

Creates a new InlineValueText object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) | The document line where to show the inline value. |
| `text` | `string` | The value to be shown for the line. |

#### Defined in

[index.d.ts:2944](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L2944)

## Properties

### range

• `Readonly` **range**: [`Range`](codearts_plugin_.Range.md)

The document range for which the inline value applies.

#### Defined in

[index.d.ts:2933](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L2933)

___

### text

• `Readonly` **text**: `string`

The text of the inline value.

#### Defined in

[index.d.ts:2937](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L2937)
