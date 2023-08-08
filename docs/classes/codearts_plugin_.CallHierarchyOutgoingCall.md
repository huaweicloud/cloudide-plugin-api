[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CallHierarchyOutgoingCall

# Class: CallHierarchyOutgoingCall

["@codearts/plugin"](../modules/_codearts_plugin_.md).CallHierarchyOutgoingCall

Represents an outgoing call, e.g. calling a getter from a method or a method from a constructor etc.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.CallHierarchyOutgoingCall.md#constructor)

### Properties

- [fromRanges](codearts_plugin_.CallHierarchyOutgoingCall.md#fromranges)
- [to](codearts_plugin_.CallHierarchyOutgoingCall.md#to)

## Constructors

### constructor

• **new CallHierarchyOutgoingCall**(`item`, `fromRanges`)

Create a new call object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`CallHierarchyItem`](codearts_plugin_.CallHierarchyItem.md) | The item being called |
| `fromRanges` | [`Range`](codearts_plugin_.Range.md)[] | The ranges at which the calls appear. |

#### Defined in

[index.d.ts:5287](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5287)

## Properties

### fromRanges

• **fromRanges**: [`Range`](codearts_plugin_.Range.md)[]

The range at which this item is called. This is the range relative to the caller, e.g the item
passed to [`provideCallHierarchyOutgoingCalls`](../interfaces/codearts_plugin_.CallHierarchyProvider.md#providecallhierarchyoutgoingcalls)
and not [`this.to`](codearts_plugin_.CallHierarchyOutgoingCall.md#to).

#### Defined in

[index.d.ts:5279](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5279)

___

### to

• **to**: [`CallHierarchyItem`](codearts_plugin_.CallHierarchyItem.md)

The item that is called.

#### Defined in

[index.d.ts:5272](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5272)
