[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / AuthenticationSession

# Interface: AuthenticationSession

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).AuthenticationSession

Represents a session of a currently logged in user.

## Table of contents

### Properties

- [accessToken](cloudide_plugin_.AuthenticationSession.md#accesstoken)
- [account](cloudide_plugin_.AuthenticationSession.md#account)
- [id](cloudide_plugin_.AuthenticationSession.md#id)
- [scopes](cloudide_plugin_.AuthenticationSession.md#scopes)

## Properties

### accessToken

• `Readonly` **accessToken**: `string`

The access token.

#### Defined in

[index.d.ts:11292](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11292)

___

### account

• `Readonly` **account**: [`AuthenticationSessionAccountInformation`](cloudide_plugin_.AuthenticationSessionAccountInformation.md)

The account associated with the session.

#### Defined in

[index.d.ts:11297](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11297)

___

### id

• `Readonly` **id**: `string`

The identifier of the authentication session.

#### Defined in

[index.d.ts:11287](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11287)

___

### scopes

• `Readonly` **scopes**: readonly `string`[]

The permissions granted by the session's access token. Available scopes
are defined by the [AuthenticationProvider](#AuthenticationProvider).

#### Defined in

[index.d.ts:11303](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11303)
