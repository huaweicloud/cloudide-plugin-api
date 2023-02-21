[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SourceBreakpoint

# Class: SourceBreakpoint

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SourceBreakpoint

A breakpoint specified by a source location.

## Hierarchy

- [`Breakpoint`](cloudide_plugin_.Breakpoint.md)

  ↳ **`SourceBreakpoint`**

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.SourceBreakpoint.md#constructor)

### Properties

- [condition](cloudide_plugin_.SourceBreakpoint.md#condition)
- [enabled](cloudide_plugin_.SourceBreakpoint.md#enabled)
- [hitCondition](cloudide_plugin_.SourceBreakpoint.md#hitcondition)
- [id](cloudide_plugin_.SourceBreakpoint.md#id)
- [location](cloudide_plugin_.SourceBreakpoint.md#location)
- [logMessage](cloudide_plugin_.SourceBreakpoint.md#logmessage)

## Constructors

### constructor

• **new SourceBreakpoint**(`location`, `enabled?`, `condition?`, `hitCondition?`, `logMessage?`)

Create a new breakpoint for a source location.

#### Parameters

| Name | Type |
| :------ | :------ |
| `location` | [`Location`](cloudide_plugin_.Location.md) |
| `enabled?` | `boolean` |
| `condition?` | `string` |
| `hitCondition?` | `string` |
| `logMessage?` | `string` |

#### Overrides

[Breakpoint](cloudide_plugin_.Breakpoint.md).[constructor](cloudide_plugin_.Breakpoint.md#constructor)

#### Defined in

[index.d.ts:10001](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10001)

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

### location

• `Readonly` **location**: [`Location`](cloudide_plugin_.Location.md)

The source and line position of this breakpoint.

#### Defined in

[index.d.ts:9996](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9996)

___

### logMessage

• `Optional` `Readonly` **logMessage**: `string`

An optional message that gets logged when this breakpoint is hit. Embedded expressions within {} are interpolated by the debug adapter.

#### Inherited from

[Breakpoint](cloudide_plugin_.Breakpoint.md).[logMessage](cloudide_plugin_.Breakpoint.md#logmessage)

#### Defined in

[index.d.ts:9984](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9984)
