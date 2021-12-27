**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / AuthenticationGetSessionOptions

# Interface: AuthenticationGetSessionOptions

Options to be used when getting an [AuthenticationSession](#AuthenticationSession) from an [AuthenticationProvider](#AuthenticationProvider).

## Hierarchy

* **AuthenticationGetSessionOptions**

## Index

### Properties

* [clearSessionPreference](_index_d_._plugin_.authenticationgetsessionoptions.md#clearsessionpreference)
* [createIfNone](_index_d_._plugin_.authenticationgetsessionoptions.md#createifnone)

## Properties

### clearSessionPreference

• `Optional` **clearSessionPreference**: boolean

*Defined in [index.d.ts:12569](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L12569)*

Whether the existing user session preference should be cleared.

For authentication providers that support being signed into multiple accounts at once, the user will be
prompted to select an account to use when [getSession](#authentication.getSession) is called. This preference
is remembered until [getSession](#authentication.getSession) is called with this flag.

Defaults to false.

___

### createIfNone

• `Optional` **createIfNone**: boolean

*Defined in [index.d.ts:12558](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L12558)*

Whether login should be performed if there is no matching session.

If true, a modal dialog will be shown asking the user to sign in. If false, a numbered badge will be shown
on the accounts activity bar icon. An entry for the extension will be added under the menu to sign in. This
allows quietly prompting the user to sign in.

Defaults to false.
