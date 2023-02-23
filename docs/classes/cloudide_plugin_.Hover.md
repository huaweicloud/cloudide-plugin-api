[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Hover

# Class: Hover

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Hover

A hover represents additional information for a symbol or word. Hovers are
rendered in a tooltip-like widget.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.Hover.md#constructor)

### Properties

- [contents](cloudide_plugin_.Hover.md#contents)
- [range](cloudide_plugin_.Hover.md#range)

## Constructors

### constructor

• **new Hover**(`contents`, `range?`)

Creates a new hover object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `contents` | [`MarkedString`](../modules/_cloudide_plugin_.md#markedstring) \| [`MarkedString`](../modules/_cloudide_plugin_.md#markedstring)[] | The contents of the hover. |
| `range?` | [`Range`](cloudide_plugin_.Range.md) | The range to which the hover applies. |

#### Defined in

[index.d.ts:9224](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9224)

## Properties

### contents

• **contents**: [`MarkedString`](../modules/_cloudide_plugin_.md#markedstring)[]

The contents of this hover.

#### Defined in

[index.d.ts:9209](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9209)

___

### range

• `Optional` **range**: [`Range`](cloudide_plugin_.Range.md)

The range to which this hover applies. When missing, the
editor will use the range at the current position or the
current position itself.

#### Defined in

[index.d.ts:9216](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9216)
