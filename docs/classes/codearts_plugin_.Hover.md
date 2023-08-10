[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Hover

# Class: Hover

["@codearts/plugin"](../modules/_codearts_plugin_.md).Hover

A hover represents additional information for a symbol or word. Hovers are
rendered in a tooltip-like widget.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.Hover.md#constructor)

### Properties

- [contents](codearts_plugin_.Hover.md#contents)
- [range](codearts_plugin_.Hover.md#range)

## Constructors

### constructor

• **new Hover**(`contents`, `range?`)

Creates a new hover object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `contents` | [`MarkdownString`](codearts_plugin_.MarkdownString.md) \| [`MarkedString`](../modules/_codearts_plugin_.md#markedstring) \| ([`MarkdownString`](codearts_plugin_.MarkdownString.md) \| [`MarkedString`](../modules/_codearts_plugin_.md#markedstring))[] | The contents of the hover. |
| `range?` | [`Range`](codearts_plugin_.Range.md) | The range to which the hover applies. |

#### Defined in

[index.d.ts:2854](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L2854)

## Properties

### contents

• **contents**: ([`MarkdownString`](codearts_plugin_.MarkdownString.md) \| [`MarkedString`](../modules/_codearts_plugin_.md#markedstring))[]

The contents of this hover.

#### Defined in

[index.d.ts:2839](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L2839)

___

### range

• `Optional` **range**: [`Range`](codearts_plugin_.Range.md)

The range to which this hover applies. When missing, the
editor will use the range at the current position or the
current position itself.

#### Defined in

[index.d.ts:2846](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L2846)
