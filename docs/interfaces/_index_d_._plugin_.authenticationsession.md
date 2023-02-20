**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / AuthenticationSession

# Interface: AuthenticationSession

Represents a session of a currently logged in user.

## Hierarchy

* **AuthenticationSession**

## Index

### Properties

* [accessToken](_index_d_._plugin_.authenticationsession.md#accesstoken)
* [account](_index_d_._plugin_.authenticationsession.md#account)
* [id](_index_d_._plugin_.authenticationsession.md#id)
* [scopes](_index_d_._plugin_.authenticationsession.md#scopes)

## Properties

### accessToken

• `Readonly` **accessToken**: string

*Defined in [index.d.ts:12515](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L12515)*

The access token.

___

### account

• `Readonly` **account**: [AuthenticationSessionAccountInformation](_index_d_._plugin_.authenticationsessionaccountinformation.md)

*Defined in [index.d.ts:12520](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L12520)*

The account associated with the session.

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:12510](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L12510)*

The identifier of the authentication session.

___

### scopes

• `Readonly` **scopes**: ReadonlyArray\<string>

*Defined in [index.d.ts:12526](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L12526)*

The permissions granted by the session's access token. Available scopes
are defined by the [AuthenticationProvider](#AuthenticationProvider).
