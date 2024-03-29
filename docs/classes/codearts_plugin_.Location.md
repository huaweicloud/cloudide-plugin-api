[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Location

# Class: Location

["@codearts/plugin"](../modules/_codearts_plugin_.md).Location

Represents a location inside a resource, such as a line
inside a text file.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.Location.md#constructor)

### Properties

- [range](codearts_plugin_.Location.md#range)
- [uri](codearts_plugin_.Location.md#uri)

## Constructors

### constructor

• **new Location**(`uri`, `rangeOrPosition`)

Creates a new location object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) | The resource identifier. |
| `rangeOrPosition` | [`Range`](codearts_plugin_.Range.md) \| [`Position`](codearts_plugin_.Position.md) | The range or position. Positions will be converted to an empty range. |

#### Defined in

[index.d.ts:5893](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5893)

## Properties

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

The document range of this location.

#### Defined in

[index.d.ts:5885](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5885)

___

### uri

• **uri**: [`Uri`](codearts_plugin_.Uri.md)

The resource identifier of this location.

#### Defined in

[index.d.ts:5880](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5880)
