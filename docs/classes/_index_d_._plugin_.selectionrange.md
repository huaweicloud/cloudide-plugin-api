**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SelectionRange

# Class: SelectionRange

A selection range represents a part of a selection hierarchy. A selection range
may have a parent selection range that contains it.

## Hierarchy

* **SelectionRange**

## Index

### Constructors

* [constructor](_index_d_._plugin_.selectionrange.md#constructor)

### Properties

* [parent](_index_d_._plugin_.selectionrange.md#parent)
* [range](_index_d_._plugin_.selectionrange.md#range)

## Constructors

### constructor

\+ **new SelectionRange**(`range`: [Range](_index_d_._plugin_.range.md), `parent?`: [SelectionRange](_index_d_._plugin_.selectionrange.md)): [SelectionRange](_index_d_._plugin_.selectionrange.md)

*Defined in [index.d.ts:4508](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4508)*

Creates a new selection range.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`range` | [Range](_index_d_._plugin_.range.md) | The range of the selection range. |
`parent?` | [SelectionRange](_index_d_._plugin_.selectionrange.md) | The parent of the selection range.  |

**Returns:** [SelectionRange](_index_d_._plugin_.selectionrange.md)

## Properties

### parent

• `Optional` **parent**: [SelectionRange](_index_d_._plugin_.selectionrange.md)

*Defined in [index.d.ts:4508](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4508)*

The parent selection range containing this range.

___

### range

•  **range**: [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:4503](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4503)*

The [range](#Range) of this selection range.
