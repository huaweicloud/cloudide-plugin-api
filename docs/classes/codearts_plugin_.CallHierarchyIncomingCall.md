[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CallHierarchyIncomingCall

# Class: CallHierarchyIncomingCall

["@codearts/plugin"](../modules/_codearts_plugin_.md).CallHierarchyIncomingCall

Represents an incoming call, e.g. a caller of a method or constructor.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.CallHierarchyIncomingCall.md#constructor)

### Properties

- [from](codearts_plugin_.CallHierarchyIncomingCall.md#from)
- [fromRanges](codearts_plugin_.CallHierarchyIncomingCall.md#fromranges)

## Constructors

### constructor

• **new CallHierarchyIncomingCall**(`item`, `fromRanges`)

Create a new call object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`CallHierarchyItem`](codearts_plugin_.CallHierarchyItem.md) | The item making the call. |
| `fromRanges` | [`Range`](codearts_plugin_.Range.md)[] | The ranges at which the calls appear. |

#### Defined in

[index.d.ts:5274](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5274)

## Properties

### from

• **from**: [`CallHierarchyItem`](codearts_plugin_.CallHierarchyItem.md)

The item that makes the call.

#### Defined in

[index.d.ts:5260](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5260)

___

### fromRanges

• **fromRanges**: [`Range`](codearts_plugin_.Range.md)[]

The range at which at which the calls appears. This is relative to the caller
denoted by [`this.from`](codearts_plugin_.CallHierarchyIncomingCall.md#from).

#### Defined in

[index.d.ts:5266](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5266)
