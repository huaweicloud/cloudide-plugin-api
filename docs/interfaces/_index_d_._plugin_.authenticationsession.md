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

*Defined in [index.d.ts:12495](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L12495)*

The access token.

___

### account

• `Readonly` **account**: [AuthenticationSessionAccountInformation](_index_d_._plugin_.authenticationsessionaccountinformation.md)

*Defined in [index.d.ts:12500](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L12500)*

The account associated with the session.

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:12490](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L12490)*

The identifier of the authentication session.

___

### scopes

• `Readonly` **scopes**: ReadonlyArray\<string>

*Defined in [index.d.ts:12506](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L12506)*

The permissions granted by the session's access token. Available scopes
are defined by the [AuthenticationProvider](#AuthenticationProvider).