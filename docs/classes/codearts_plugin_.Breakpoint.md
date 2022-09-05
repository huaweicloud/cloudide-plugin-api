[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Breakpoint

# Class: Breakpoint

["@codearts/plugin"](../modules/_codearts_plugin_.md).Breakpoint

The base class of all breakpoint types.

## Hierarchy

- **`Breakpoint`**

  ↳ [`SourceBreakpoint`](codearts_plugin_.SourceBreakpoint.md)

  ↳ [`FunctionBreakpoint`](codearts_plugin_.FunctionBreakpoint.md)

## Table of contents

### Constructors

- [constructor](codearts_plugin_.Breakpoint.md#constructor)

### Properties

- [condition](codearts_plugin_.Breakpoint.md#condition)
- [enabled](codearts_plugin_.Breakpoint.md#enabled)
- [hitCondition](codearts_plugin_.Breakpoint.md#hitcondition)
- [id](codearts_plugin_.Breakpoint.md#id)
- [logMessage](codearts_plugin_.Breakpoint.md#logmessage)

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

[index.d.ts:14512](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14512)

## Properties

### condition

• `Optional` `Readonly` **condition**: `string`

An optional expression for conditional breakpoints.

#### Defined in

[index.d.ts:14502](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14502)

___

### enabled

• `Readonly` **enabled**: `boolean`

Is breakpoint enabled.

#### Defined in

[index.d.ts:14498](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14498)

___

### hitCondition

• `Optional` `Readonly` **hitCondition**: `string`

An optional expression that controls how many hits of the breakpoint are ignored.

#### Defined in

[index.d.ts:14506](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14506)

___

### id

• `Readonly` **id**: `string`

The unique ID of the breakpoint.

#### Defined in

[index.d.ts:14494](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14494)

___

### logMessage

• `Optional` `Readonly` **logMessage**: `string`

An optional message that gets logged when this breakpoint is hit. Embedded expressions within {} are interpolated by the debug adapter.

#### Defined in

[index.d.ts:14510](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14510)
