[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / FunctionBreakpoint

# Class: FunctionBreakpoint

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).FunctionBreakpoint

A breakpoint specified by a function name.

## Hierarchy

- [`Breakpoint`](cloudide_plugin_.Breakpoint.md)

  ↳ **`FunctionBreakpoint`**

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.FunctionBreakpoint.md#constructor)

### Properties

- [condition](cloudide_plugin_.FunctionBreakpoint.md#condition)
- [enabled](cloudide_plugin_.FunctionBreakpoint.md#enabled)
- [functionName](cloudide_plugin_.FunctionBreakpoint.md#functionname)
- [hitCondition](cloudide_plugin_.FunctionBreakpoint.md#hitcondition)
- [id](cloudide_plugin_.FunctionBreakpoint.md#id)
- [logMessage](cloudide_plugin_.FunctionBreakpoint.md#logmessage)

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

[Breakpoint](cloudide_plugin_.Breakpoint.md).[constructor](cloudide_plugin_.Breakpoint.md#constructor)

#### Defined in

[index.d.ts:10016](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10016)

## Properties

### condition

• `Optional` `Readonly` **condition**: `string`

An optional expression for conditional breakpoints.

#### Inherited from

[Breakpoint](cloudide_plugin_.Breakpoint.md).[condition](cloudide_plugin_.Breakpoint.md#condition)

#### Defined in

[index.d.ts:9976](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9976)

___

### enabled

• `Readonly` **enabled**: `boolean`

Is breakpoint enabled.

#### Inherited from

[Breakpoint](cloudide_plugin_.Breakpoint.md).[enabled](cloudide_plugin_.Breakpoint.md#enabled)

#### Defined in

[index.d.ts:9972](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9972)

___

### functionName

• `Readonly` **functionName**: `string`

The name of the function to which this breakpoint is attached.

#### Defined in

[index.d.ts:10011](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10011)

___

### hitCondition

• `Optional` `Readonly` **hitCondition**: `string`

An optional expression that controls how many hits of the breakpoint are ignored.

#### Inherited from

[Breakpoint](cloudide_plugin_.Breakpoint.md).[hitCondition](cloudide_plugin_.Breakpoint.md#hitcondition)

#### Defined in

[index.d.ts:9980](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9980)

___

### id

• `Readonly` **id**: `string`

The unique ID of the breakpoint.

#### Inherited from

[Breakpoint](cloudide_plugin_.Breakpoint.md).[id](cloudide_plugin_.Breakpoint.md#id)

#### Defined in

[index.d.ts:9968](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9968)

___

### logMessage

• `Optional` `Readonly` **logMessage**: `string`

An optional message that gets logged when this breakpoint is hit. Embedded expressions within {} are interpolated by the debug adapter.

#### Inherited from

[Breakpoint](cloudide_plugin_.Breakpoint.md).[logMessage](cloudide_plugin_.Breakpoint.md#logmessage)

#### Defined in

[index.d.ts:9984](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9984)
