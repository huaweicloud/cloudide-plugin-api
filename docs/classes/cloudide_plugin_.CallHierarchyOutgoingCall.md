[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CallHierarchyOutgoingCall

# Class: CallHierarchyOutgoingCall

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CallHierarchyOutgoingCall

Represents an outgoing call, e.g. calling a getter from a method or a method from a constructor etc.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.CallHierarchyOutgoingCall.md#constructor)

### Properties

- [fromRanges](cloudide_plugin_.CallHierarchyOutgoingCall.md#fromranges)
- [to](cloudide_plugin_.CallHierarchyOutgoingCall.md#to)

## Constructors

### constructor

• **new CallHierarchyOutgoingCall**(`item`, `fromRanges`)

Create a new call object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`CallHierarchyItem`](cloudide_plugin_.CallHierarchyItem.md) | The item being called |
| `fromRanges` | [`Range`](cloudide_plugin_.Range.md)[] | The ranges at which the calls appear. |

#### Defined in

[index.d.ts:11232](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11232)

## Properties

### fromRanges

• **fromRanges**: [`Range`](cloudide_plugin_.Range.md)[]

The range at which this item is called. This is the range relative to the caller, e.g the item
passed to [`provideCallHierarchyOutgoingCalls`](#CallHierarchyItemProvider.provideCallHierarchyOutgoingCalls)
and not [`this.to`](#CallHierarchyOutgoingCall.to).

#### Defined in

[index.d.ts:11224](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11224)

___

### to

• **to**: [`CallHierarchyItem`](cloudide_plugin_.CallHierarchyItem.md)

The item that is called.

#### Defined in

[index.d.ts:11217](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11217)
