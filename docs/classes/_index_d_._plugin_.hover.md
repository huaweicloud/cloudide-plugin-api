**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Hover

# Class: Hover

A hover represents additional information for a symbol or word. Hovers are
rendered in a tooltip-like widget.

## Hierarchy

* **Hover**

## Index

### Constructors

* [constructor](_index_d_._plugin_.hover.md#constructor)

### Properties

* [contents](_index_d_._plugin_.hover.md#contents)
* [range](_index_d_._plugin_.hover.md#range)

## Constructors

### constructor

\+ **new Hover**(`contents`: [MarkedString](../modules/_index_d_._plugin_.md#markedstring) \| [MarkedString](../modules/_index_d_._plugin_.md#markedstring)[], `range?`: [Range](_index_d_._plugin_.range.md)): [Hover](_index_d_._plugin_.hover.md)

*Defined in [index.d.ts:2708](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2708)*

Creates a new hover object.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`contents` | [MarkedString](../modules/_index_d_._plugin_.md#markedstring) \| [MarkedString](../modules/_index_d_._plugin_.md#markedstring)[] | The contents of the hover. |
`range?` | [Range](_index_d_._plugin_.range.md) | The range to which the hover applies.  |

**Returns:** [Hover](_index_d_._plugin_.hover.md)

## Properties

### contents

•  **contents**: [MarkedString](../modules/_index_d_._plugin_.md#markedstring)[]

*Defined in [index.d.ts:2701](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2701)*

The contents of this hover.

___

### range

• `Optional` **range**: [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:2708](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2708)*

The range to which this hover applies. When missing, the
editor will use the range at the current position or the
current position itself.
