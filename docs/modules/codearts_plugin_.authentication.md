[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / authentication

# Namespace: authentication

["@codearts/plugin"](_codearts_plugin_.md).authentication

Namespace for authentication.

## Table of contents

### Functions

- [getSession](codearts_plugin_.authentication.md#getsession)
- [onDidChangeSessions](codearts_plugin_.authentication.md#ondidchangesessions)
- [registerAuthenticationProvider](codearts_plugin_.authentication.md#registerauthenticationprovider)

## Functions

### getSession

▸ **getSession**(`providerId`, `scopes`, `options`): [`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/codearts_plugin_.AuthenticationSession.md)\>

Get an authentication session matching the desired scopes. Rejects if a provider with providerId is not
registered, or if the user does not consent to sharing authentication information with
the extension. If there are multiple sessions with the same scopes, the user will be shown a
quickpick to select which account they would like to use.

Currently, there are only two authentication providers that are contributed from built in extensions
to the editor that implement GitHub and Microsoft authentication: their providerId's are 'github' and 'microsoft'.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `providerId` | `string` | The id of the provider to use |
| `scopes` | readonly `string`[] | A list of scopes representing the permissions requested. These are dependent on the authentication provider |
| `options` | [`AuthenticationGetSessionOptions`](../interfaces/codearts_plugin_.AuthenticationGetSessionOptions.md) & { `createIfNone`: ``true``  } | The [AuthenticationGetSessionOptions](../interfaces/codearts_plugin_.AuthenticationGetSessionOptions.md) to use |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/codearts_plugin_.AuthenticationSession.md)\>

A thenable that resolves to an authentication session

#### Defined in

[index.d.ts:15315](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15315)

▸ **getSession**(`providerId`, `scopes`, `options`): [`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/codearts_plugin_.AuthenticationSession.md)\>

Get an authentication session matching the desired scopes. Rejects if a provider with providerId is not
registered, or if the user does not consent to sharing authentication information with
the extension. If there are multiple sessions with the same scopes, the user will be shown a
quickpick to select which account they would like to use.

Currently, there are only two authentication providers that are contributed from built in extensions
to the editor that implement GitHub and Microsoft authentication: their providerId's are 'github' and 'microsoft'.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `providerId` | `string` | The id of the provider to use |
| `scopes` | readonly `string`[] | A list of scopes representing the permissions requested. These are dependent on the authentication provider |
| `options` | [`AuthenticationGetSessionOptions`](../interfaces/codearts_plugin_.AuthenticationGetSessionOptions.md) & { `forceNewSession`: ``true`` \| { `detail`: `string`  }  } | The [AuthenticationGetSessionOptions](../interfaces/codearts_plugin_.AuthenticationGetSessionOptions.md) to use |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/codearts_plugin_.AuthenticationSession.md)\>

A thenable that resolves to an authentication session

#### Defined in

[index.d.ts:15330](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15330)

▸ **getSession**(`providerId`, `scopes`, `options?`): [`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/codearts_plugin_.AuthenticationSession.md) \| `undefined`\>

Get an authentication session matching the desired scopes. Rejects if a provider with providerId is not
registered, or if the user does not consent to sharing authentication information with
the extension. If there are multiple sessions with the same scopes, the user will be shown a
quickpick to select which account they would like to use.

Currently, there are only two authentication providers that are contributed from built in extensions
to the editor that implement GitHub and Microsoft authentication: their providerId's are 'github' and 'microsoft'.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `providerId` | `string` | The id of the provider to use |
| `scopes` | readonly `string`[] | A list of scopes representing the permissions requested. These are dependent on the authentication provider |
| `options?` | [`AuthenticationGetSessionOptions`](../interfaces/codearts_plugin_.AuthenticationGetSessionOptions.md) | The [AuthenticationGetSessionOptions](../interfaces/codearts_plugin_.AuthenticationGetSessionOptions.md) to use |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/codearts_plugin_.AuthenticationSession.md) \| `undefined`\>

A thenable that resolves to an authentication session if available, or undefined if there are no sessions

#### Defined in

[index.d.ts:15345](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15345)

___

### onDidChangeSessions

▸ **onDidChangeSessions**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`AuthenticationSessionsChangeEvent`](../interfaces/codearts_plugin_.AuthenticationSessionsChangeEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1603)

___

### registerAuthenticationProvider

▸ **registerAuthenticationProvider**(`id`, `label`, `provider`, `options?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register an authentication provider.

There can only be one provider per id and an error is being thrown when an id
has already been used by another provider. Ids are case-sensitive.

**`Params`**

options Additional options for the provider.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | The unique identifier of the provider. |
| `label` | `string` | The human-readable name of the provider. |
| `provider` | [`AuthenticationProvider`](../interfaces/codearts_plugin_.AuthenticationProvider.md) | The authentication provider provider. |
| `options?` | [`AuthenticationProviderOptions`](../interfaces/codearts_plugin_.AuthenticationProviderOptions.md) | - |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:15365](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15365)
