[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / authentication

# Namespace: authentication

["@codearts/plugin"](_codearts_plugin_.md).authentication

## Table of contents

### Functions

- [getSession](codearts_plugin_.authentication.md#getsession)
- [onDidChangeSessions](codearts_plugin_.authentication.md#ondidchangesessions)
- [registerAuthenticationProvider](codearts_plugin_.authentication.md#registerauthenticationprovider)

## Functions

### getSession

▸ **getSession**(`providerId`, `scopes`, `options`): [`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/codearts_plugin_.AuthenticationSession.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `providerId` | `string` |  |
| `scopes` | readonly `string`[] |  |
| `options` | [`AuthenticationGetSessionOptions`](../interfaces/codearts_plugin_.AuthenticationGetSessionOptions.md) & { `createIfNone`: ``true``  } |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/codearts_plugin_.AuthenticationSession.md)\>

#### Defined in

[index.d.ts:15223](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L15223)

▸ **getSession**(`providerId`, `scopes`, `options`): [`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/codearts_plugin_.AuthenticationSession.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `providerId` | `string` |  |
| `scopes` | readonly `string`[] |  |
| `options` | [`AuthenticationGetSessionOptions`](../interfaces/codearts_plugin_.AuthenticationGetSessionOptions.md) & { `forceNewSession`: ``true`` \| { `detail`: `string`  }  } |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/codearts_plugin_.AuthenticationSession.md)\>

#### Defined in

[index.d.ts:15238](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L15238)

▸ **getSession**(`providerId`, `scopes`, `options?`): [`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/codearts_plugin_.AuthenticationSession.md) \| `undefined`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `providerId` | `string` |  |
| `scopes` | readonly `string`[] |  |
| `options?` | [`AuthenticationGetSessionOptions`](../interfaces/codearts_plugin_.AuthenticationGetSessionOptions.md) |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`AuthenticationSession`](../interfaces/codearts_plugin_.AuthenticationSession.md) \| `undefined`\>

#### Defined in

[index.d.ts:15253](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L15253)

___

### onDidChangeSessions

▸ `Const` **onDidChangeSessions**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`AuthenticationSessionsChangeEvent`](../interfaces/codearts_plugin_.AuthenticationSessionsChangeEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:15259](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L15259)

___

### registerAuthenticationProvider

▸ **registerAuthenticationProvider**(`id`, `label`, `provider`, `options?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` |  |
| `label` | `string` |  |
| `provider` | [`AuthenticationProvider`](../interfaces/codearts_plugin_.AuthenticationProvider.md) |  |
| `options?` | [`AuthenticationProviderOptions`](../interfaces/codearts_plugin_.AuthenticationProviderOptions.md) | - |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:15273](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L15273)
