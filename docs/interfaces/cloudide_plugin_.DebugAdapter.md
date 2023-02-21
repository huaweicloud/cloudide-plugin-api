[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DebugAdapter

# Interface: DebugAdapter

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DebugAdapter

A debug adapter that implements the Debug Adapter Protocol can be registered with the editor if it implements the DebugAdapter interface.

## Hierarchy

- [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

  ↳ **`DebugAdapter`**

## Table of contents

### Properties

- [onDidSendMessage](cloudide_plugin_.DebugAdapter.md#ondidsendmessage)

### Methods

- [dispose](cloudide_plugin_.DebugAdapter.md#dispose)
- [handleMessage](cloudide_plugin_.DebugAdapter.md#handlemessage)

## Properties

### onDidSendMessage

• `Readonly` **onDidSendMessage**: [`Event`](cloudide_plugin_.Event.md)<[`DebugProtocolMessage`](cloudide_plugin_.DebugProtocolMessage.md)\>

An event which fires after the debug adapter has sent a Debug Adapter Protocol message to the editor.
Messages can be requests, responses, or events.

#### Defined in

[index.d.ts:9860](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9860)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose this object.

#### Returns

`void`

#### Inherited from

[Disposable](../classes/cloudide_plugin_.Disposable.md).[dispose](../classes/cloudide_plugin_.Disposable.md#dispose)

#### Defined in

[index.d.ts:27](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L27)

___

### handleMessage

▸ **handleMessage**(`message`): `void`

Handle a Debug Adapter Protocol message.
Messages can be requests, responses, or events.
Results or errors are returned via onSendMessage events.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | [`DebugProtocolMessage`](cloudide_plugin_.DebugProtocolMessage.md) | A Debug Adapter Protocol message |

#### Returns

`void`

#### Defined in

[index.d.ts:9868](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9868)
