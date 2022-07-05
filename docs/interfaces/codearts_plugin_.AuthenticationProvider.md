[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / AuthenticationProvider

# Interface: AuthenticationProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).AuthenticationProvider

## Table of contents

### Properties

- [onDidChangeSessions](codearts_plugin_.AuthenticationProvider.md#ondidchangesessions)

### Methods

- [createSession](codearts_plugin_.AuthenticationProvider.md#createsession)
- [getSessions](codearts_plugin_.AuthenticationProvider.md#getsessions)
- [removeSession](codearts_plugin_.AuthenticationProvider.md#removesession)

## Properties

### onDidChangeSessions

• `Readonly` **onDidChangeSessions**: [`Event`](codearts_plugin_.Event.md)<[`AuthenticationProviderAuthenticationSessionsChangeEvent`](codearts_plugin_.AuthenticationProviderAuthenticationSessionsChangeEvent.md)\>

#### Defined in

[index.d.ts:15169](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L15169)

## Methods

### createSession

▸ **createSession**(`scopes`): [`Thenable`](Thenable.md)<[`AuthenticationSession`](codearts_plugin_.AuthenticationSession.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scopes` | readonly `string`[] |  |

#### Returns

[`Thenable`](Thenable.md)<[`AuthenticationSession`](codearts_plugin_.AuthenticationSession.md)\>

#### Defined in

[index.d.ts:15192](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L15192)

___

### getSessions

▸ **getSessions**(`scopes?`): [`Thenable`](Thenable.md)<readonly [`AuthenticationSession`](codearts_plugin_.AuthenticationSession.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scopes?` | readonly `string`[] |  |

#### Returns

[`Thenable`](Thenable.md)<readonly [`AuthenticationSession`](codearts_plugin_.AuthenticationSession.md)[]\>

#### Defined in

[index.d.ts:15177](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L15177)

___

### removeSession

▸ **removeSession**(`sessionId`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sessionId` | `string` |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:15202](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L15202)
