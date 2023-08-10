[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / AuthenticationProviderAuthenticationSessionsChangeEvent

# Interface: AuthenticationProviderAuthenticationSessionsChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).AuthenticationProviderAuthenticationSessionsChangeEvent

An [Event](codearts_plugin_.Event.md) which fires when an [AuthenticationSession](codearts_plugin_.AuthenticationSession.md) is added, removed, or changed.

## Table of contents

### Properties

- [added](codearts_plugin_.AuthenticationProviderAuthenticationSessionsChangeEvent.md#added)
- [changed](codearts_plugin_.AuthenticationProviderAuthenticationSessionsChangeEvent.md#changed)
- [removed](codearts_plugin_.AuthenticationProviderAuthenticationSessionsChangeEvent.md#removed)

## Properties

### added

• `Readonly` **added**: `undefined` \| readonly [`AuthenticationSession`](codearts_plugin_.AuthenticationSession.md)[]

The [AuthenticationSessions](codearts_plugin_.AuthenticationSession.md) of the [AuthenticationProvider](codearts_plugin_.AuthenticationProvider.md) that have been added.

#### Defined in

[index.d.ts:16165](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16165)

___

### changed

• `Readonly` **changed**: `undefined` \| readonly [`AuthenticationSession`](codearts_plugin_.AuthenticationSession.md)[]

The [AuthenticationSessions](codearts_plugin_.AuthenticationSession.md) of the [AuthenticationProvider](codearts_plugin_.AuthenticationProvider.md) that have been changed.
A session changes when its data excluding the id are updated. An example of this is a session refresh that results in a new
access token being set for the session.

#### Defined in

[index.d.ts:16177](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16177)

___

### removed

• `Readonly` **removed**: `undefined` \| readonly [`AuthenticationSession`](codearts_plugin_.AuthenticationSession.md)[]

The [AuthenticationSessions](codearts_plugin_.AuthenticationSession.md) of the [AuthenticationProvider](codearts_plugin_.AuthenticationProvider.md) that have been removed.

#### Defined in

[index.d.ts:16170](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16170)
