[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / AuthenticationProvider

# Interface: AuthenticationProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).AuthenticationProvider

A provider for performing authentication to a service.

## Table of contents

### Properties

- [onDidChangeSessions](codearts_plugin_.AuthenticationProvider.md#ondidchangesessions)

### Methods

- [createSession](codearts_plugin_.AuthenticationProvider.md#createsession)
- [getSessions](codearts_plugin_.AuthenticationProvider.md#getsessions)
- [getSignHeaders](codearts_plugin_.AuthenticationProvider.md#getsignheaders)
- [removeSession](codearts_plugin_.AuthenticationProvider.md#removesession)

## Properties

### onDidChangeSessions

• `Readonly` **onDidChangeSessions**: [`Event`](codearts_plugin_.Event.md)<[`AuthenticationProviderAuthenticationSessionsChangeEvent`](codearts_plugin_.AuthenticationProviderAuthenticationSessionsChangeEvent.md)\>

An [Event](codearts_plugin_.Event.md) which fires when the array of sessions has changed, or data
within a session has changed.

#### Defined in

[index.d.ts:15621](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15621)

## Methods

### createSession

▸ **createSession**(`scopes`): [`Thenable`](Thenable.md)<[`AuthenticationSession`](codearts_plugin_.AuthenticationSession.md)\>

Prompts a user to login.

If login is successful, the onDidChangeSessions event should be fired.

If login fails, a rejected promise should be returned.

If the provider has specified that it does not support multiple accounts,
then this should never be called if there is already an existing session matching these
scopes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scopes` | readonly `string`[] | A list of scopes, permissions, that the new session should be created with. |

#### Returns

[`Thenable`](Thenable.md)<[`AuthenticationSession`](codearts_plugin_.AuthenticationSession.md)\>

A promise that resolves to an authentication session.

#### Defined in

[index.d.ts:15644](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15644)

___

### getSessions

▸ **getSessions**(`scopes?`): [`Thenable`](Thenable.md)<readonly [`AuthenticationSession`](codearts_plugin_.AuthenticationSession.md)[]\>

Get a list of sessions.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scopes?` | readonly `string`[] | An optional list of scopes. If provided, the sessions returned should match these permissions, otherwise all sessions should be returned. |

#### Returns

[`Thenable`](Thenable.md)<readonly [`AuthenticationSession`](codearts_plugin_.AuthenticationSession.md)[]\>

A promise that resolves to an array of authentication sessions.

#### Defined in

[index.d.ts:15629](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15629)

___

### getSignHeaders

▸ `Optional` **getSignHeaders**(`options`): [`Thenable`](Thenable.md)<`undefined` \| [`SignedHeaders`](codearts_plugin_.SignedHeaders.md)\>

Provide a signed http request header.

Can use own crypto function to implement it.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`SignRequestOptions`](codearts_plugin_.SignRequestOptions.md) | The params of http request to sign. |

#### Returns

[`Thenable`](Thenable.md)<`undefined` \| [`SignedHeaders`](codearts_plugin_.SignedHeaders.md)\>

#### Defined in

[index.d.ts:15662](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15662)

___

### removeSession

▸ **removeSession**(`sessionId`): [`Thenable`](Thenable.md)<`void`\>

Removes the session corresponding to session id.

If the removal is successful, the onDidChangeSessions event should be fired.

If a session cannot be removed, the provider should reject with an error message.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sessionId` | `string` | The id of the session to remove. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:15654](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15654)
