[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / AuthenticationSession

# Interface: AuthenticationSession

["@codearts/plugin"](../modules/_codearts_plugin_.md).AuthenticationSession

Represents a session of a currently logged in user.

## Table of contents

### Properties

- [accessToken](codearts_plugin_.AuthenticationSession.md#accesstoken)
- [account](codearts_plugin_.AuthenticationSession.md#account)
- [id](codearts_plugin_.AuthenticationSession.md#id)
- [scopes](codearts_plugin_.AuthenticationSession.md#scopes)

## Properties

### accessToken

• `Readonly` **accessToken**: `string`

The access token.

#### Defined in

[index.d.ts:15831](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15831)

___

### account

• `Readonly` **account**: [`AuthenticationSessionAccountInformation`](codearts_plugin_.AuthenticationSessionAccountInformation.md)

The account associated with the session.

#### Defined in

[index.d.ts:15836](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15836)

___

### id

• `Readonly` **id**: `string`

The identifier of the authentication session.

#### Defined in

[index.d.ts:15826](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15826)

___

### scopes

• `Readonly` **scopes**: readonly `string`[]

The permissions granted by the session's access token. Available scopes
are defined by the [AuthenticationProvider](codearts_plugin_.AuthenticationProvider.md).

#### Defined in

[index.d.ts:15842](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L15842)
