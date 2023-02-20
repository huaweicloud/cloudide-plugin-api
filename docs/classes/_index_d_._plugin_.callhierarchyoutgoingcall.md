**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CallHierarchyOutgoingCall

# Class: CallHierarchyOutgoingCall

Represents an outgoing call, e.g. calling a getter from a method or a method from a constructor etc.

## Hierarchy

* **CallHierarchyOutgoingCall**

## Index

### Constructors

* [constructor](_index_d_._plugin_.callhierarchyoutgoingcall.md#constructor)

### Properties

* [fromRanges](_index_d_._plugin_.callhierarchyoutgoingcall.md#fromranges)
* [to](_index_d_._plugin_.callhierarchyoutgoingcall.md#to)

## Constructors

### constructor

\+ **new CallHierarchyOutgoingCall**(`item`: [CallHierarchyItem](_index_d_._plugin_.callhierarchyitem.md), `fromRanges`: [Range](_index_d_._plugin_.range.md)[]): [CallHierarchyOutgoingCall](_index_d_._plugin_.callhierarchyoutgoingcall.md)

*Defined in [index.d.ts:4623](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4623)*

Create a new call object.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`item` | [CallHierarchyItem](_index_d_._plugin_.callhierarchyitem.md) | The item being called |
`fromRanges` | [Range](_index_d_._plugin_.range.md)[] | The ranges at which the calls appear.  |

**Returns:** [CallHierarchyOutgoingCall](_index_d_._plugin_.callhierarchyoutgoingcall.md)

## Properties

### fromRanges

•  **fromRanges**: [Range](_index_d_._plugin_.range.md)[]

*Defined in [index.d.ts:4623](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4623)*

The range at which this item is called. This is the range relative to the caller, e.g the item
passed to [`provideCallHierarchyOutgoingCalls`](#CallHierarchyProvider.provideCallHierarchyOutgoingCalls)
and not [`this.to`](#CallHierarchyOutgoingCall.to).

___

### to

•  **to**: [CallHierarchyItem](_index_d_._plugin_.callhierarchyitem.md)

*Defined in [index.d.ts:4616](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L4616)*

The item that is called.
