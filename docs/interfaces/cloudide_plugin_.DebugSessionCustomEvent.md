[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DebugSessionCustomEvent

# Interface: DebugSessionCustomEvent

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DebugSessionCustomEvent

A custom Debug Adapter Protocol event received from a [debug session](#DebugSession).

## Table of contents

### Properties

- [body](cloudide_plugin_.DebugSessionCustomEvent.md#body)
- [event](cloudide_plugin_.DebugSessionCustomEvent.md#event)
- [session](cloudide_plugin_.DebugSessionCustomEvent.md#session)

## Properties

### body

• `Optional` **body**: `any`

Event specific information.

#### Defined in

[index.d.ts:9642](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9642)

___

### event

• **event**: `string`

Type of event.

#### Defined in

[index.d.ts:9637](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9637)

___

### session

• **session**: [`DebugSession`](cloudide_plugin_.DebugSession.md)

The [debug session](#DebugSession) for which the custom event was received.

#### Defined in

[index.d.ts:9632](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9632)
