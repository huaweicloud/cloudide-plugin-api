[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugAdapter

# Interface: DebugAdapter

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugAdapter

A debug adapter that implements the Debug Adapter Protocol can be registered with the editor if it implements the DebugAdapter interface.

## Hierarchy

- [`Disposable`](../classes/codearts_plugin_.Disposable.md)

  ↳ **`DebugAdapter`**

## Table of contents

### Properties

- [onDidSendMessage](codearts_plugin_.DebugAdapter.md#ondidsendmessage)

### Methods

- [dispose](codearts_plugin_.DebugAdapter.md#dispose)
- [handleMessage](codearts_plugin_.DebugAdapter.md#handlemessage)

## Properties

### onDidSendMessage

• `Readonly` **onDidSendMessage**: [`Event`](codearts_plugin_.Event.md)<[`DebugProtocolMessage`](codearts_plugin_.DebugProtocolMessage.md)\>

An event which fires after the debug adapter has sent a Debug Adapter Protocol message to the editor.
Messages can be requests, responses, or events.

#### Defined in

[index.d.ts:15268](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15268)

## Methods

### dispose

▸ **dispose**(): `any`

Dispose this object.

#### Returns

`any`

#### Inherited from

[Disposable](../classes/codearts_plugin_.Disposable.md).[dispose](../classes/codearts_plugin_.Disposable.md#dispose)

#### Defined in

[index.d.ts:1580](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L1580)

___

### handleMessage

▸ **handleMessage**(`message`): `void`

Handle a Debug Adapter Protocol message.
Messages can be requests, responses, or events.
Results or errors are returned via onSendMessage events.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | [`DebugProtocolMessage`](codearts_plugin_.DebugProtocolMessage.md) | A Debug Adapter Protocol message |

#### Returns

`void`

#### Defined in

[index.d.ts:15276](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15276)
