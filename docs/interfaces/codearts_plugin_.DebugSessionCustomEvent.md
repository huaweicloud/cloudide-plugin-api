[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugSessionCustomEvent

# Interface: DebugSessionCustomEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugSessionCustomEvent

A custom Debug Adapter Protocol event received from a [debug session](codearts_plugin_.DebugSession.md).

## Table of contents

### Properties

- [body](codearts_plugin_.DebugSessionCustomEvent.md#body)
- [event](codearts_plugin_.DebugSessionCustomEvent.md#event)
- [session](codearts_plugin_.DebugSessionCustomEvent.md#session)

## Properties

### body

• `Readonly` **body**: `any`

Event specific information.

#### Defined in

[index.d.ts:15094](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L15094)

___

### event

• `Readonly` **event**: `string`

Type of event.

#### Defined in

[index.d.ts:15089](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L15089)

___

### session

• `Readonly` **session**: [`DebugSession`](codearts_plugin_.DebugSession.md)

The [debug session](codearts_plugin_.DebugSession.md) for which the custom event was received.

#### Defined in

[index.d.ts:15084](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L15084)
