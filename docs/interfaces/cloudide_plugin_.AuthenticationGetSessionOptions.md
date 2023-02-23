[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / AuthenticationGetSessionOptions

# Interface: AuthenticationGetSessionOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).AuthenticationGetSessionOptions

Options to be used when getting an [AuthenticationSession](#AuthenticationSession) from an [AuthenticationProvider](#AuthenticationProvider).

## Table of contents

### Properties

- [clearSessionPreference](cloudide_plugin_.AuthenticationGetSessionOptions.md#clearsessionpreference)
- [createIfNone](cloudide_plugin_.AuthenticationGetSessionOptions.md#createifnone)

## Properties

### clearSessionPreference

• `Optional` **clearSessionPreference**: `boolean`

Whether the existing user session preference should be cleared.

For authentication providers that support being signed into multiple accounts at once, the user will be
prompted to select an account to use when [getSession](#authentication.getSession) is called. This preference
is remembered until [getSession](#authentication.getSession) is called with this flag.

Defaults to false.

#### Defined in

[index.d.ts:11345](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11345)

___

### createIfNone

• `Optional` **createIfNone**: `boolean`

Whether login should be performed if there is no matching session.

If true, a modal dialog will be shown asking the user to sign in. If false, a numbered badge will be shown
on the accounts activity bar icon. An entry for the extension will be added under the menu to sign in. This
allows quietly prompting the user to sign in.

Defaults to false.

#### Defined in

[index.d.ts:11334](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11334)
