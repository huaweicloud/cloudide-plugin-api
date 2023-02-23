[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DebugAdapterTracker

# Interface: DebugAdapterTracker

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DebugAdapterTracker

A Debug Adapter Tracker is a means to track the communication between VS Code and a Debug Adapter.

## Table of contents

### Methods

- [onDidSendMessage](cloudide_plugin_.DebugAdapterTracker.md#ondidsendmessage)
- [onError](cloudide_plugin_.DebugAdapterTracker.md#onerror)
- [onExit](cloudide_plugin_.DebugAdapterTracker.md#onexit)
- [onWillReceiveMessage](cloudide_plugin_.DebugAdapterTracker.md#onwillreceivemessage)
- [onWillStartSession](cloudide_plugin_.DebugAdapterTracker.md#onwillstartsession)
- [onWillStopSession](cloudide_plugin_.DebugAdapterTracker.md#onwillstopsession)

## Methods

### onDidSendMessage

▸ `Optional` **onDidSendMessage**(`message`): `void`

The debug adapter has sent a Debug Adapter Protocol message to VS Code.

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `any` |

#### Returns

`void`

#### Defined in

[index.d.ts:9738](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9738)

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

[index.d.ts:9746](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9746)

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

[index.d.ts:9750](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9750)

___

### onWillReceiveMessage

▸ `Optional` **onWillReceiveMessage**(`message`): `void`

The debug adapter is about to receive a Debug Adapter Protocol message from VS Code.

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `any` |

#### Returns

`void`

#### Defined in

[index.d.ts:9734](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9734)

___

### onWillStartSession

▸ `Optional` **onWillStartSession**(): `void`

A session with the debug adapter is about to be started.

#### Returns

`void`

#### Defined in

[index.d.ts:9730](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9730)

___

### onWillStopSession

▸ `Optional` **onWillStopSession**(): `void`

The debug adapter session is about to be stopped.

#### Returns

`void`

#### Defined in

[index.d.ts:9742](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9742)
