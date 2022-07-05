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

[index.d.ts:14329](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L14329)

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

[index.d.ts:14337](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L14337)

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

[index.d.ts:14341](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L14341)

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

[index.d.ts:14325](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L14325)

___

### onWillStartSession

▸ `Optional` **onWillStartSession**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:14321](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L14321)

___

### onWillStopSession

▸ `Optional` **onWillStopSession**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:14333](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L14333)
