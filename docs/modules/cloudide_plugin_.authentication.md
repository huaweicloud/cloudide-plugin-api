[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](_cloudide_plugin_.md) / authentication

# Namespace: authentication

["@cloudide/plugin"](_cloudide_plugin_.md).authentication

Namespace for authentication.

## Table of contents

### Functions

- [getSession](cloudide_plugin_.authentication.md#getsession)
- [onDidChangeSessions](cloudide_plugin_.authentication.md#ondidchangesessions)

## Functions

### getSession

▸ **getSession**(`providerId`, `scopes`, `options`): [`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/cloudide_plugin_.AuthenticationSession.md)\>

Get an authentication session matching the desired scopes. Rejects if a provider with providerId is not
registered, or if the user does not consent to sharing authentication information with
the extension. If there are multiple sessions with the same scopes, the user will be shown a
quickpick to select which account they would like to use.

Currently, there are only two authentication providers that are contributed from built in extensions
to VS Code that implement GitHub and Microsoft authentication: their providerId's are 'github' and 'microsoft'.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `providerId` | `string` | The id of the provider to use |
| `scopes` | `string`[] | A list of scopes representing the permissions requested. These are dependent on the authentication provider |
| `options` | [`AuthenticationGetSessionOptions`](../interfaces/cloudide_plugin_.AuthenticationGetSessionOptions.md) & { `createIfNone`: ``true``  } | The [getSessionOptions](#GetSessionOptions) to use |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/cloudide_plugin_.AuthenticationSession.md)\>

A thenable that resolves to an authentication session

#### Defined in

[index.d.ts:11390](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11390)

▸ **getSession**(`providerId`, `scopes`, `options?`): [`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/cloudide_plugin_.AuthenticationSession.md) \| `undefined`\>

Get an authentication session matching the desired scopes. Rejects if a provider with providerId is not
registered, or if the user does not consent to sharing authentication information with
the extension. If there are multiple sessions with the same scopes, the user will be shown a
quickpick to select which account they would like to use.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `providerId` | `string` | The id of the provider to use |
| `scopes` | `string`[] | A list of scopes representing the permissions requested. These are dependent on the authentication provider |
| `options?` | [`AuthenticationGetSessionOptions`](../interfaces/cloudide_plugin_.AuthenticationGetSessionOptions.md) | The [getSessionOptions](#GetSessionOptions) to use |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/cloudide_plugin_.AuthenticationSession.md) \| `undefined`\>

A thenable that resolves to an authentication session if available, or undefined if there are no sessions

#### Defined in

[index.d.ts:11403](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11403)

___

### onDidChangeSessions

▸ **onDidChangeSessions**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`AuthenticationSessionsChangeEvent`](../interfaces/cloudide_plugin_.AuthenticationSessionsChangeEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)
