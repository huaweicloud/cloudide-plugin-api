**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SourceBreakpoint

# Class: SourceBreakpoint

A breakpoint specified by a source location.

## Hierarchy

* [Breakpoint](_index_d_._plugin_.breakpoint.md)

  ↳ **SourceBreakpoint**

## Index

### Constructors

* [constructor](_index_d_._plugin_.sourcebreakpoint.md#constructor)

### Properties

* [condition](_index_d_._plugin_.sourcebreakpoint.md#condition)
* [enabled](_index_d_._plugin_.sourcebreakpoint.md#enabled)
* [hitCondition](_index_d_._plugin_.sourcebreakpoint.md#hitcondition)
* [id](_index_d_._plugin_.sourcebreakpoint.md#id)
* [location](_index_d_._plugin_.sourcebreakpoint.md#location)
* [logMessage](_index_d_._plugin_.sourcebreakpoint.md#logmessage)

## Constructors

### constructor

\+ **new SourceBreakpoint**(`location`: [Location](_index_d_._plugin_.location.md), `enabled?`: boolean, `condition?`: string, `hitCondition?`: string, `logMessage?`: string): [SourceBreakpoint](_index_d_._plugin_.sourcebreakpoint.md)

*Overrides [Breakpoint](_index_d_._plugin_.breakpoint.md).[constructor](_index_d_._plugin_.breakpoint.md#constructor)*

*Defined in [index.d.ts:10464](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10464)*

Create a new breakpoint for a source location.

#### Parameters:

Name | Type |
------ | ------ |
`location` | [Location](_index_d_._plugin_.location.md) |
`enabled?` | boolean |
`condition?` | string |
`hitCondition?` | string |
`logMessage?` | string |

**Returns:** [SourceBreakpoint](_index_d_._plugin_.sourcebreakpoint.md)

## Properties

### condition

• `Optional` `Readonly` **condition**: string

*Inherited from [Breakpoint](_index_d_._plugin_.breakpoint.md).[condition](_index_d_._plugin_.breakpoint.md#condition)*

*Defined in [index.d.ts:10444](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10444)*

An optional expression for conditional breakpoints.

___

### enabled

• `Readonly` **enabled**: boolean

*Inherited from [Breakpoint](_index_d_._plugin_.breakpoint.md).[enabled](_index_d_._plugin_.breakpoint.md#enabled)*

*Defined in [index.d.ts:10440](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10440)*

Is breakpoint enabled.

___

### hitCondition

• `Optional` `Readonly` **hitCondition**: string

*Inherited from [Breakpoint](_index_d_._plugin_.breakpoint.md).[hitCondition](_index_d_._plugin_.breakpoint.md#hitcondition)*

*Defined in [index.d.ts:10448](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10448)*

An optional expression that controls how many hits of the breakpoint are ignored.

___

### id

• `Readonly` **id**: string

*Inherited from [Breakpoint](_index_d_._plugin_.breakpoint.md).[id](_index_d_._plugin_.breakpoint.md#id)*

*Defined in [index.d.ts:10436](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10436)*

The unique ID of the breakpoint.

___

### location

• `Readonly` **location**: [Location](_index_d_._plugin_.location.md)

*Defined in [index.d.ts:10464](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10464)*

The source and line position of this breakpoint.

___

### logMessage

• `Optional` `Readonly` **logMessage**: string

*Inherited from [Breakpoint](_index_d_._plugin_.breakpoint.md).[logMessage](_index_d_._plugin_.breakpoint.md#logmessage)*

*Defined in [index.d.ts:10452](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10452)*

An optional message that gets logged when this breakpoint is hit. Embedded expressions within {} are interpolated by the debug adapter.
