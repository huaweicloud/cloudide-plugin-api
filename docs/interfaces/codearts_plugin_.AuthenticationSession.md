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

[index.d.ts:15108](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15108)

___

### account

• `Readonly` **account**: [`AuthenticationSessionAccountInformation`](codearts_plugin_.AuthenticationSessionAccountInformation.md)

The account associated with the session.

#### Defined in

[index.d.ts:15113](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15113)

___

### id

• `Readonly` **id**: `string`

The identifier of the authentication session.

#### Defined in

[index.d.ts:15103](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15103)

___

### scopes

• `Readonly` **scopes**: readonly `string`[]

The permissions granted by the session's access token. Available scopes
are defined by the [AuthenticationProvider](codearts_plugin_.AuthenticationProvider.md).

#### Defined in

[index.d.ts:15119](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L15119)
