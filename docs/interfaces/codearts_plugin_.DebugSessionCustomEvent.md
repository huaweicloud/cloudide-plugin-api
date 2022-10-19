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

[index.d.ts:14382](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14382)

___

### event

• `Readonly` **event**: `string`

Type of event.

#### Defined in

[index.d.ts:14377](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14377)

___

### session

• `Readonly` **session**: [`DebugSession`](codearts_plugin_.DebugSession.md)

The [debug session](codearts_plugin_.DebugSession.md) for which the custom event was received.

#### Defined in

[index.d.ts:14372](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L14372)
