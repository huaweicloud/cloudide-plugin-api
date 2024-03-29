[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SourceBreakpoint

# Class: SourceBreakpoint

["@codearts/plugin"](../modules/_codearts_plugin_.md).SourceBreakpoint

A breakpoint specified by a source location.

## Hierarchy

- [`Breakpoint`](codearts_plugin_.Breakpoint.md)

  ↳ **`SourceBreakpoint`**

## Table of contents

### Constructors

- [constructor](codearts_plugin_.SourceBreakpoint.md#constructor)

### Properties

- [condition](codearts_plugin_.SourceBreakpoint.md#condition)
- [enabled](codearts_plugin_.SourceBreakpoint.md#enabled)
- [hitCondition](codearts_plugin_.SourceBreakpoint.md#hitcondition)
- [id](codearts_plugin_.SourceBreakpoint.md#id)
- [location](codearts_plugin_.SourceBreakpoint.md#location)
- [logMessage](codearts_plugin_.SourceBreakpoint.md#logmessage)

## Constructors

### constructor

• **new SourceBreakpoint**(`location`, `enabled?`, `condition?`, `hitCondition?`, `logMessage?`)

Create a new breakpoint for a source location.

#### Parameters

| Name | Type |
| :------ | :------ |
| `location` | [`Location`](codearts_plugin_.Location.md) |
| `enabled?` | `boolean` |
| `condition?` | `string` |
| `hitCondition?` | `string` |
| `logMessage?` | `string` |

#### Overrides

[Breakpoint](codearts_plugin_.Breakpoint.md).[constructor](codearts_plugin_.Breakpoint.md#constructor)

#### Defined in

[index.d.ts:15434](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15434)

## Properties

### condition

• `Optional` `Readonly` **condition**: `string`

An optional expression for conditional breakpoints.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[condition](codearts_plugin_.Breakpoint.md#condition)

#### Defined in

[index.d.ts:15409](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15409)

___

### enabled

• `Readonly` **enabled**: `boolean`

Is breakpoint enabled.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[enabled](codearts_plugin_.Breakpoint.md#enabled)

#### Defined in

[index.d.ts:15405](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15405)

___

### hitCondition

• `Optional` `Readonly` **hitCondition**: `string`

An optional expression that controls how many hits of the breakpoint are ignored.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[hitCondition](codearts_plugin_.Breakpoint.md#hitcondition)

#### Defined in

[index.d.ts:15413](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15413)

___

### id

• `Readonly` **id**: `string`

The unique ID of the breakpoint.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[id](codearts_plugin_.Breakpoint.md#id)

#### Defined in

[index.d.ts:15401](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15401)

___

### location

• `Readonly` **location**: [`Location`](codearts_plugin_.Location.md)

The source and line position of this breakpoint.

#### Defined in

[index.d.ts:15429](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15429)

___

### logMessage

• `Optional` `Readonly` **logMessage**: `string`

An optional message that gets logged when this breakpoint is hit. Embedded expressions within {} are interpolated by the debug adapter.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[logMessage](codearts_plugin_.Breakpoint.md#logmessage)

#### Defined in

[index.d.ts:15417](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15417)
