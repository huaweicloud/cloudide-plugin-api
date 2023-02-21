[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CallHierarchyIncomingCall

# Class: CallHierarchyIncomingCall

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CallHierarchyIncomingCall

Represents an incoming call, e.g. a caller of a method or constructor.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.CallHierarchyIncomingCall.md#constructor)

### Properties

- [from](cloudide_plugin_.CallHierarchyIncomingCall.md#from)
- [fromRanges](cloudide_plugin_.CallHierarchyIncomingCall.md#fromranges)

## Constructors

### constructor

• **new CallHierarchyIncomingCall**(`item`, `fromRanges`)

Create a new call object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`CallHierarchyItem`](cloudide_plugin_.CallHierarchyItem.md) | The item making the call. |
| `fromRanges` | [`Range`](cloudide_plugin_.Range.md)[] | The ranges at which the calls appear. |

#### Defined in

[index.d.ts:11206](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11206)

## Properties

### from

• **from**: [`CallHierarchyItem`](cloudide_plugin_.CallHierarchyItem.md)

The item that makes the call.

#### Defined in

[index.d.ts:11192](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11192)

___

### fromRanges

• **fromRanges**: [`Range`](cloudide_plugin_.Range.md)[]

The range at which at which the calls appears. This is relative to the caller
denoted by [`this.from`](#CallHierarchyIncomingCall.from).

#### Defined in

[index.d.ts:11198](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11198)
