[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugAdapter

# Interface: DebugAdapter

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugAdapter

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

#### Defined in

[index.d.ts:14269](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14269)

## Methods

### dispose

▸ **dispose**(): `any`

#### Returns

`any`

#### Inherited from

[Disposable](../classes/codearts_plugin_.Disposable.md).[dispose](../classes/codearts_plugin_.Disposable.md#dispose)

#### Defined in

[index.d.ts:1580](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L1580)

___

### handleMessage

▸ **handleMessage**(`message`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | [`DebugProtocolMessage`](codearts_plugin_.DebugProtocolMessage.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:14277](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L14277)
