[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Breakpoint

# Class: Breakpoint

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Breakpoint

The base class of all breakpoint types.

## Hierarchy

- **`Breakpoint`**

  ↳ [`SourceBreakpoint`](cloudide_plugin_.SourceBreakpoint.md)

  ↳ [`FunctionBreakpoint`](cloudide_plugin_.FunctionBreakpoint.md)

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.Breakpoint.md#constructor)

### Properties

- [condition](cloudide_plugin_.Breakpoint.md#condition)
- [enabled](cloudide_plugin_.Breakpoint.md#enabled)
- [hitCondition](cloudide_plugin_.Breakpoint.md#hitcondition)
- [id](cloudide_plugin_.Breakpoint.md#id)
- [logMessage](cloudide_plugin_.Breakpoint.md#logmessage)

## Constructors

### constructor

• `Protected` **new Breakpoint**(`enabled?`, `condition?`, `hitCondition?`, `logMessage?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled?` | `boolean` |
| `condition?` | `string` |
| `hitCondition?` | `string` |
| `logMessage?` | `string` |

#### Defined in

[index.d.ts:9986](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9986)

## Properties

### condition

• `Optional` `Readonly` **condition**: `string`

An optional expression for conditional breakpoints.

#### Defined in

[index.d.ts:9976](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9976)

___

### enabled

• `Readonly` **enabled**: `boolean`

Is breakpoint enabled.

#### Defined in

[index.d.ts:9972](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9972)

___

### hitCondition

• `Optional` `Readonly` **hitCondition**: `string`

An optional expression that controls how many hits of the breakpoint are ignored.

#### Defined in

[index.d.ts:9980](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9980)

___

### id

• `Readonly` **id**: `string`

The unique ID of the breakpoint.

#### Defined in

[index.d.ts:9968](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9968)

___

### logMessage

• `Optional` `Readonly` **logMessage**: `string`

An optional message that gets logged when this breakpoint is hit. Embedded expressions within {} are interpolated by the debug adapter.

#### Defined in

[index.d.ts:9984](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9984)
