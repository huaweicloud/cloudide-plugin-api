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

[index.d.ts:16035](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16035)

___

### account

• `Readonly` **account**: [`AuthenticationSessionAccountInformation`](codearts_plugin_.AuthenticationSessionAccountInformation.md)

The account associated with the session.

#### Defined in

[index.d.ts:16040](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16040)

___

### id

• `Readonly` **id**: `string`

The identifier of the authentication session.

#### Defined in

[index.d.ts:16030](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16030)

___

### scopes

• `Readonly` **scopes**: readonly `string`[]

The permissions granted by the session's access token. Available scopes
are defined by the [AuthenticationProvider](codearts_plugin_.AuthenticationProvider.md).

#### Defined in

[index.d.ts:16046](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16046)
