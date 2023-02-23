[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Location

# Class: Location

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Location

Represents a location inside a resource, such as a line
inside a text file.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.Location.md#constructor)

### Properties

- [range](cloudide_plugin_.Location.md#range)
- [uri](cloudide_plugin_.Location.md#uri)

## Constructors

### constructor

• **new Location**(`uri`, `rangeOrPosition`)

Creates a new location object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](cloudide_plugin_.Uri.md) | The resource identifier. |
| `rangeOrPosition` | [`Position`](cloudide_plugin_.Position.md) \| [`Range`](cloudide_plugin_.Range.md) | The range or position. Positions will be converted to an empty range. |

#### Defined in

[index.d.ts:7689](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7689)

## Properties

### range

• **range**: [`Range`](cloudide_plugin_.Range.md)

The document range of this location.

#### Defined in

[index.d.ts:7681](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7681)

___

### uri

• **uri**: [`Uri`](cloudide_plugin_.Uri.md)

The resource identifier of this location.

#### Defined in

[index.d.ts:7676](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7676)
