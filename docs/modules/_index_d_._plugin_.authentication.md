**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](_index_d_.md) / ["plugin"](_index_d_._plugin_.md) / authentication

# Namespace: authentication

Namespace for authentication.

## Index

### Variables

* [onDidChangeSessions](_index_d_._plugin_.authentication.md#ondidchangesessions)

### Functions

* [getSession](_index_d_._plugin_.authentication.md#getsession)

## Variables

### onDidChangeSessions

• `Const` **onDidChangeSessions**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[AuthenticationSessionsChangeEvent](../interfaces/_index_d_._plugin_.authenticationsessionschangeevent.md)>

*Defined in [index.d.ts:12635](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L12635)*

An [event](#Event) which fires when the authentication sessions of an authentication provider have
been added, removed, or changed.

## Functions

### getSession

▸ **getSession**(`providerId`: string, `scopes`: string[], `options`: [AuthenticationGetSessionOptions](../interfaces/_index_d_._plugin_.authenticationgetsessionoptions.md) & { createIfNone: true  }): [Thenable](../interfaces/_index_d_.thenable.md)\<[AuthenticationSession](../interfaces/_index_d_._plugin_.authenticationsession.md)>

*Defined in [index.d.ts:12614](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L12614)*

Get an authentication session matching the desired scopes. Rejects if a provider with providerId is not
registered, or if the user does not consent to sharing authentication information with
the extension. If there are multiple sessions with the same scopes, the user will be shown a
quickpick to select which account they would like to use.

Currently, there are only two authentication providers that are contributed from built in extensions
to VS Code that implement GitHub and Microsoft authentication: their providerId's are 'github' and 'microsoft'.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`providerId` | string | The id of the provider to use |
`scopes` | string[] | A list of scopes representing the permissions requested. These are dependent on the authentication provider |
`options` | [AuthenticationGetSessionOptions](../interfaces/_index_d_._plugin_.authenticationgetsessionoptions.md) & { createIfNone: true  } | The [getSessionOptions](#GetSessionOptions) to use |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[AuthenticationSession](../interfaces/_index_d_._plugin_.authenticationsession.md)>

A thenable that resolves to an authentication session

▸ **getSession**(`providerId`: string, `scopes`: string[], `options?`: [AuthenticationGetSessionOptions](../interfaces/_index_d_._plugin_.authenticationgetsessionoptions.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<[AuthenticationSession](../interfaces/_index_d_._plugin_.authenticationsession.md) \| undefined>

*Defined in [index.d.ts:12629](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L12629)*

Get an authentication session matching the desired scopes. Rejects if a provider with providerId is not
registered, or if the user does not consent to sharing authentication information with
the extension. If there are multiple sessions with the same scopes, the user will be shown a
quickpick to select which account they would like to use.

Currently, there are only two authentication providers that are contributed from built in extensions
to VS Code that implement GitHub and Microsoft authentication: their providerId's are 'github' and 'microsoft'.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`providerId` | string | The id of the provider to use |
`scopes` | string[] | A list of scopes representing the permissions requested. These are dependent on the authentication provider |
`options?` | [AuthenticationGetSessionOptions](../interfaces/_index_d_._plugin_.authenticationgetsessionoptions.md) | The [getSessionOptions](#GetSessionOptions) to use |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[AuthenticationSession](../interfaces/_index_d_._plugin_.authenticationsession.md) \| undefined>

A thenable that resolves to an authentication session if available, or undefined if there are no sessions
