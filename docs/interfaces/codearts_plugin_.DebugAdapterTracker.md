[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugAdapterTracker

# Interface: DebugAdapterTracker

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugAdapterTracker

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

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `any` |

#### Returns

`void`

#### Defined in

[index.d.ts:14359](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14359)

___

### onError

▸ `Optional` **onError**(`error`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `error` | `Error` |

#### Returns

`void`

#### Defined in

[index.d.ts:14367](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14367)

___

### onExit

▸ `Optional` **onExit**(`code`, `signal`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `code` | `undefined` \| `number` |
| `signal` | `undefined` \| `string` |

#### Returns

`void`

#### Defined in

[index.d.ts:14371](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14371)

___

### onWillReceiveMessage

▸ `Optional` **onWillReceiveMessage**(`message`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `any` |

#### Returns

`void`

#### Defined in

[index.d.ts:14355](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14355)

___

### onWillStartSession

▸ `Optional` **onWillStartSession**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:14351](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14351)

___

### onWillStopSession

▸ `Optional` **onWillStopSession**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:14363](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14363)
