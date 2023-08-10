[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugAdapterTracker

# Interface: DebugAdapterTracker

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugAdapterTracker

A Debug Adapter Tracker is a means to track the communication between the editor and a Debug Adapter.

## Table of contents

### Methods

- [onDidSendMessage](codearts_plugin_.DebugAdapterTracker.md#ondidsendmessage)
- [onError](codearts_plugin_.DebugAdapterTracker.md#onerror)
- [onExit](codearts_plugin_.DebugAdapterTracker.md#onexit)
- [onWillReceiveMessage](codearts_plugin_.DebugAdapterTracker.md#onwillreceivemessage)
- [onWillStartSession](codearts_plugin_.DebugAdapterTracker.md#onwillstartsession)
- [onWillStopSession](codearts_plugin_.DebugAdapterTracker.md#onwillstopsession)

## Methods

### onDidSendMessage

▸ `Optional` **onDidSendMessage**(`message`): `void`

The debug adapter has sent a Debug Adapter Protocol message to the editor.

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `any` |

#### Returns

`void`

#### Defined in

[index.d.ts:15328](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15328)

___

### onError

▸ `Optional` **onError**(`error`): `void`

An error with the debug adapter has occurred.

#### Parameters

| Name | Type |
| :------ | :------ |
| `error` | `Error` |

#### Returns

`void`

#### Defined in

[index.d.ts:15336](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15336)

___

### onExit

▸ `Optional` **onExit**(`code`, `signal`): `void`

The debug adapter has exited with the given exit code or signal.

#### Parameters

| Name | Type |
| :------ | :------ |
| `code` | `undefined` \| `number` |
| `signal` | `undefined` \| `string` |

#### Returns

`void`

#### Defined in

[index.d.ts:15340](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15340)

___

### onWillReceiveMessage

▸ `Optional` **onWillReceiveMessage**(`message`): `void`

The debug adapter is about to receive a Debug Adapter Protocol message from the editor.

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `any` |

#### Returns

`void`

#### Defined in

[index.d.ts:15324](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15324)

___

### onWillStartSession

▸ `Optional` **onWillStartSession**(): `void`

A session with the debug adapter is about to be started.

#### Returns

`void`

#### Defined in

[index.d.ts:15320](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15320)

___

### onWillStopSession

▸ `Optional` **onWillStopSession**(): `void`

The debug adapter session is about to be stopped.

#### Returns

`void`

#### Defined in

[index.d.ts:15332](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15332)
