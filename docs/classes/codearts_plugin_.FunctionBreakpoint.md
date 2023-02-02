[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FunctionBreakpoint

# Class: FunctionBreakpoint

["@codearts/plugin"](../modules/_codearts_plugin_.md).FunctionBreakpoint

A breakpoint specified by a function name.

## Hierarchy

- [`Breakpoint`](codearts_plugin_.Breakpoint.md)

  ↳ **`FunctionBreakpoint`**

## Table of contents

### Constructors

- [constructor](codearts_plugin_.FunctionBreakpoint.md#constructor)

### Properties

- [condition](codearts_plugin_.FunctionBreakpoint.md#condition)
- [enabled](codearts_plugin_.FunctionBreakpoint.md#enabled)
- [functionName](codearts_plugin_.FunctionBreakpoint.md#functionname)
- [hitCondition](codearts_plugin_.FunctionBreakpoint.md#hitcondition)
- [id](codearts_plugin_.FunctionBreakpoint.md#id)
- [logMessage](codearts_plugin_.FunctionBreakpoint.md#logmessage)

## Constructors

### constructor

• **new FunctionBreakpoint**(`functionName`, `enabled?`, `condition?`, `hitCondition?`, `logMessage?`)

Create a new function breakpoint.

#### Parameters

| Name | Type |
| :------ | :------ |
| `functionName` | `string` |
| `enabled?` | `boolean` |
| `condition?` | `string` |
| `hitCondition?` | `string` |
| `logMessage?` | `string` |

#### Overrides

[Breakpoint](codearts_plugin_.Breakpoint.md).[constructor](codearts_plugin_.Breakpoint.md#constructor)

#### Defined in

[index.d.ts:15265](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15265)

## Properties

### condition

• `Optional` `Readonly` **condition**: `string`

An optional expression for conditional breakpoints.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[condition](codearts_plugin_.Breakpoint.md#condition)

#### Defined in

[index.d.ts:15225](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15225)

___

### enabled

• `Readonly` **enabled**: `boolean`

Is breakpoint enabled.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[enabled](codearts_plugin_.Breakpoint.md#enabled)

#### Defined in

[index.d.ts:15221](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15221)

___

### functionName

• `Readonly` **functionName**: `string`

The name of the function to which this breakpoint is attached.

#### Defined in

[index.d.ts:15260](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15260)

___

### hitCondition

• `Optional` `Readonly` **hitCondition**: `string`

An optional expression that controls how many hits of the breakpoint are ignored.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[hitCondition](codearts_plugin_.Breakpoint.md#hitcondition)

#### Defined in

[index.d.ts:15229](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15229)

___

### id

• `Readonly` **id**: `string`

The unique ID of the breakpoint.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[id](codearts_plugin_.Breakpoint.md#id)

#### Defined in

[index.d.ts:15217](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15217)

___

### logMessage

• `Optional` `Readonly` **logMessage**: `string`

An optional message that gets logged when this breakpoint is hit. Embedded expressions within {} are interpolated by the debug adapter.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[logMessage](codearts_plugin_.Breakpoint.md#logmessage)

#### Defined in

[index.d.ts:15233](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15233)
