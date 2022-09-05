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

[index.d.ts:14527](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14527)

## Properties

### condition

• `Optional` `Readonly` **condition**: `string`

An optional expression for conditional breakpoints.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[condition](codearts_plugin_.Breakpoint.md#condition)

#### Defined in

[index.d.ts:14502](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14502)

___

### enabled

• `Readonly` **enabled**: `boolean`

Is breakpoint enabled.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[enabled](codearts_plugin_.Breakpoint.md#enabled)

#### Defined in

[index.d.ts:14498](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14498)

___

### hitCondition

• `Optional` `Readonly` **hitCondition**: `string`

An optional expression that controls how many hits of the breakpoint are ignored.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[hitCondition](codearts_plugin_.Breakpoint.md#hitcondition)

#### Defined in

[index.d.ts:14506](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14506)

___

### id

• `Readonly` **id**: `string`

The unique ID of the breakpoint.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[id](codearts_plugin_.Breakpoint.md#id)

#### Defined in

[index.d.ts:14494](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14494)

___

### location

• `Readonly` **location**: [`Location`](codearts_plugin_.Location.md)

The source and line position of this breakpoint.

#### Defined in

[index.d.ts:14522](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14522)

___

### logMessage

• `Optional` `Readonly` **logMessage**: `string`

An optional message that gets logged when this breakpoint is hit. Embedded expressions within {} are interpolated by the debug adapter.

#### Inherited from

[Breakpoint](codearts_plugin_.Breakpoint.md).[logMessage](codearts_plugin_.Breakpoint.md#logmessage)

#### Defined in

[index.d.ts:14510](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14510)
