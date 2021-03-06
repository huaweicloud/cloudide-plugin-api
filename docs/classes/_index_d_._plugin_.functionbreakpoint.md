**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FunctionBreakpoint

# Class: FunctionBreakpoint

A breakpoint specified by a function name.

## Hierarchy

* [Breakpoint](_index_d_._plugin_.breakpoint.md)

  ↳ **FunctionBreakpoint**

## Index

### Constructors

* [constructor](_index_d_._plugin_.functionbreakpoint.md#constructor)

### Properties

* [condition](_index_d_._plugin_.functionbreakpoint.md#condition)
* [enabled](_index_d_._plugin_.functionbreakpoint.md#enabled)
* [functionName](_index_d_._plugin_.functionbreakpoint.md#functionname)
* [hitCondition](_index_d_._plugin_.functionbreakpoint.md#hitcondition)
* [id](_index_d_._plugin_.functionbreakpoint.md#id)
* [logMessage](_index_d_._plugin_.functionbreakpoint.md#logmessage)

## Constructors

### constructor

\+ **new FunctionBreakpoint**(`functionName`: string, `enabled?`: boolean, `condition?`: string, `hitCondition?`: string, `logMessage?`: string): [FunctionBreakpoint](_index_d_._plugin_.functionbreakpoint.md)

*Overrides [Breakpoint](_index_d_._plugin_.breakpoint.md).[constructor](_index_d_._plugin_.breakpoint.md#constructor)*

*Defined in [index.d.ts:10479](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10479)*

Create a new function breakpoint.

#### Parameters:

Name | Type |
------ | ------ |
`functionName` | string |
`enabled?` | boolean |
`condition?` | string |
`hitCondition?` | string |
`logMessage?` | string |

**Returns:** [FunctionBreakpoint](_index_d_._plugin_.functionbreakpoint.md)

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

### functionName

• `Readonly` **functionName**: string

*Defined in [index.d.ts:10479](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10479)*

The name of the function to which this breakpoint is attached.

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

### logMessage

• `Optional` `Readonly` **logMessage**: string

*Inherited from [Breakpoint](_index_d_._plugin_.breakpoint.md).[logMessage](_index_d_._plugin_.breakpoint.md#logmessage)*

*Defined in [index.d.ts:10452](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10452)*

An optional message that gets logged when this breakpoint is hit. Embedded expressions within {} are interpolated by the debug adapter.
