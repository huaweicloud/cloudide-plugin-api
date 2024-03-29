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

[index.d.ts:15419](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15419)

## Properties

### condition

• `Optional` `Readonly` **condition**: `string`

An optional expression for conditional breakpoints.

#### Defined in

[index.d.ts:15409](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15409)

___

### enabled

• `Readonly` **enabled**: `boolean`

Is breakpoint enabled.

#### Defined in

[index.d.ts:15405](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15405)

___

### hitCondition

• `Optional` `Readonly` **hitCondition**: `string`

An optional expression that controls how many hits of the breakpoint are ignored.

#### Defined in

[index.d.ts:15413](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15413)

___

### id

• `Readonly` **id**: `string`

The unique ID of the breakpoint.

#### Defined in

[index.d.ts:15401](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15401)

___

### logMessage

• `Optional` `Readonly` **logMessage**: `string`

An optional message that gets logged when this breakpoint is hit. Embedded expressions within {} are interpolated by the debug adapter.

#### Defined in

[index.d.ts:15417](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15417)
