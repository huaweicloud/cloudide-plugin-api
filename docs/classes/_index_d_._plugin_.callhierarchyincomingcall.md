**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CallHierarchyIncomingCall

# Class: CallHierarchyIncomingCall

Represents an incoming call, e.g. a caller of a method or constructor.

## Hierarchy

* **CallHierarchyIncomingCall**

## Index

### Constructors

* [constructor](_index_d_._plugin_.callhierarchyincomingcall.md#constructor)

### Properties

* [from](_index_d_._plugin_.callhierarchyincomingcall.md#from)
* [fromRanges](_index_d_._plugin_.callhierarchyincomingcall.md#fromranges)

## Constructors

### constructor

\+ **new CallHierarchyIncomingCall**(`item`: [CallHierarchyItem](_index_d_._plugin_.callhierarchyitem.md), `fromRanges`: [Range](_index_d_._plugin_.range.md)[]): [CallHierarchyIncomingCall](_index_d_._plugin_.callhierarchyincomingcall.md)

*Defined in [index.d.ts:4594](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4594)*

Create a new call object.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`item` | [CallHierarchyItem](_index_d_._plugin_.callhierarchyitem.md) | The item making the call. |
`fromRanges` | [Range](_index_d_._plugin_.range.md)[] | The ranges at which the calls appear.  |

**Returns:** [CallHierarchyIncomingCall](_index_d_._plugin_.callhierarchyincomingcall.md)

## Properties

### from

•  **from**: [CallHierarchyItem](_index_d_._plugin_.callhierarchyitem.md)

*Defined in [index.d.ts:4588](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4588)*

The item that makes the call.

___

### fromRanges

•  **fromRanges**: [Range](_index_d_._plugin_.range.md)[]

*Defined in [index.d.ts:4594](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4594)*

The range at which at which the calls appears. This is relative to the caller
denoted by [`this.from`](#CallHierarchyIncomingCall.from).
