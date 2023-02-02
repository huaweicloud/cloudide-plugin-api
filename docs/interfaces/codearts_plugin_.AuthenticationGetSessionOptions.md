[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / AuthenticationGetSessionOptions

# Interface: AuthenticationGetSessionOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).AuthenticationGetSessionOptions

Options to be used when getting an [AuthenticationSession](codearts_plugin_.AuthenticationSession.md) from an [AuthenticationProvider](codearts_plugin_.AuthenticationProvider.md).

## Table of contents

### Properties

- [clearSessionPreference](codearts_plugin_.AuthenticationGetSessionOptions.md#clearsessionpreference)
- [createIfNone](codearts_plugin_.AuthenticationGetSessionOptions.md#createifnone)
- [forceNewSession](codearts_plugin_.AuthenticationGetSessionOptions.md#forcenewsession)
- [silent](codearts_plugin_.AuthenticationGetSessionOptions.md#silent)

## Properties

### clearSessionPreference

• `Optional` **clearSessionPreference**: `boolean`

Whether the existing user session preference should be cleared.

For authentication providers that support being signed into multiple accounts at once, the user will be
prompted to select an account to use when [getSession](../modules/codearts_plugin_.authentication.md#getsession) is called. This preference
is remembered until [getSession](../modules/codearts_plugin_.authentication.md#getsession) is called with this flag.

Defaults to false.

#### Defined in

[index.d.ts:15874](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15874)

___

### createIfNone

• `Optional` **createIfNone**: `boolean`

Whether login should be performed if there is no matching session.

If true, a modal dialog will be shown asking the user to sign in. If false, a numbered badge will be shown
on the accounts activity bar icon. An entry for the extension will be added under the menu to sign in. This
allows quietly prompting the user to sign in.

If there is a matching session but the extension has not been granted access to it, setting this to true
will also result in an immediate modal dialog, and false will add a numbered badge to the accounts icon.

Defaults to false.

Note: you cannot use this option with [silent](codearts_plugin_.AuthenticationGetSessionOptions.md#silent).

#### Defined in

[index.d.ts:15890](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15890)

___

### forceNewSession

• `Optional` **forceNewSession**: `boolean` \| { `detail`: `string`  }

Whether we should attempt to reauthenticate even if there is already a session available.

If true, a modal dialog will be shown asking the user to sign in again. This is mostly used for scenarios
where the token needs to be re minted because it has lost some authorization.

If there are no existing sessions and forceNewSession is true, it will behave identically to
[createIfNone](codearts_plugin_.AuthenticationGetSessionOptions.md#createifnone).

This defaults to false.

#### Defined in

[index.d.ts:15903](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15903)

___

### silent

• `Optional` **silent**: `boolean`

Whether we should show the indication to sign in in the Accounts menu.

If false, the user will be shown a badge on the Accounts menu with an option to sign in for the extension.
If true, no indication will be shown.

Defaults to false.

Note: you cannot use this option with any other options that prompt the user like [createIfNone](codearts_plugin_.AuthenticationGetSessionOptions.md#createifnone).

#### Defined in

[index.d.ts:15915](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15915)
