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

[index.d.ts:5229](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L5229)

## Properties

### fromRanges

• **fromRanges**: [`Range`](codearts_plugin_.Range.md)[]

The range at which this item is called. This is the range relative to the caller, e.g the item
passed to [`provideCallHierarchyOutgoingCalls`](../interfaces/codearts_plugin_.CallHierarchyProvider.md#providecallhierarchyoutgoingcalls)
and not [`this.to`](codearts_plugin_.CallHierarchyOutgoingCall.md#to).

#### Defined in

[index.d.ts:5221](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L5221)

___

### to

• **to**: [`CallHierarchyItem`](codearts_plugin_.CallHierarchyItem.md)

The item that is called.

#### Defined in

[index.d.ts:5214](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L5214)
