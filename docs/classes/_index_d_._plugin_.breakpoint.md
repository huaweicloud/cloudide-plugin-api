**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Breakpoint

# Class: Breakpoint

The base class of all breakpoint types.

## Hierarchy

* **Breakpoint**

  ↳ [SourceBreakpoint](_index_d_._plugin_.sourcebreakpoint.md)

  ↳ [FunctionBreakpoint](_index_d_._plugin_.functionbreakpoint.md)

## Index

### Constructors

* [constructor](_index_d_._plugin_.breakpoint.md#constructor)

### Properties

* [condition](_index_d_._plugin_.breakpoint.md#condition)
* [enabled](_index_d_._plugin_.breakpoint.md#enabled)
* [hitCondition](_index_d_._plugin_.breakpoint.md#hitcondition)
* [id](_index_d_._plugin_.breakpoint.md#id)
* [logMessage](_index_d_._plugin_.breakpoint.md#logmessage)

## Constructors

### constructor

\+ `Protected`**new Breakpoint**(`enabled?`: boolean, `condition?`: string, `hitCondition?`: string, `logMessage?`: string): [Breakpoint](_index_d_._plugin_.breakpoint.md)

*Defined in [index.d.ts:10452](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10452)*

#### Parameters:

Name | Type |
------ | ------ |
`enabled?` | boolean |
`condition?` | string |
`hitCondition?` | string |
`logMessage?` | string |

**Returns:** [Breakpoint](_index_d_._plugin_.breakpoint.md)

## Properties

### condition

• `Optional` `Readonly` **condition**: string

*Defined in [index.d.ts:10444](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10444)*

An optional expression for conditional breakpoints.

___

### enabled

• `Readonly` **enabled**: boolean

*Defined in [index.d.ts:10440](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10440)*

Is breakpoint enabled.

___

### hitCondition

• `Optional` `Readonly` **hitCondition**: string

*Defined in [index.d.ts:10448](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10448)*

An optional expression that controls how many hits of the breakpoint are ignored.

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:10436](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10436)*

The unique ID of the breakpoint.

___

### logMessage

• `Optional` `Readonly` **logMessage**: string

*Defined in [index.d.ts:10452](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10452)*

An optional message that gets logged when this breakpoint is hit. Embedded expressions within {} are interpolated by the debug adapter.
