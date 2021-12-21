**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Location

# Class: Location

Represents a location inside a resource, such as a line
inside a text file.

## Hierarchy

* **Location**

## Index

### Constructors

* [constructor](_index_d_._plugin_.location.md#constructor)

### Properties

* [range](_index_d_._plugin_.location.md#range)
* [uri](_index_d_._plugin_.location.md#uri)

## Constructors

### constructor

\+ **new Location**(`uri`: [Uri](_index_d_._plugin_.uri.md), `rangeOrPosition`: [Range](_index_d_._plugin_.range.md) \| [Position](_index_d_._plugin_.position.md)): [Location](_index_d_._plugin_.location.md)

*Defined in [index.d.ts:5092](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5092)*

Creates a new location object.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](_index_d_._plugin_.uri.md) | The resource identifier. |
`rangeOrPosition` | [Range](_index_d_._plugin_.range.md) \| [Position](_index_d_._plugin_.position.md) | The range or position. Positions will be converted to an empty range.  |

**Returns:** [Location](_index_d_._plugin_.location.md)

## Properties

### range

•  **range**: [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:5092](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5092)*

The document range of this location.

___

### uri

•  **uri**: [Uri](_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:5087](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5087)*

The resource identifier of this location.
