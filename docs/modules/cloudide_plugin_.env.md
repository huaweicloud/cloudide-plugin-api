[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](_cloudide_plugin_.md) / env

# Namespace: env

["@cloudide/plugin"](_cloudide_plugin_.md).env

## Table of contents

### Variables

- [appName](cloudide_plugin_.env.md#appname)
- [appRoot](cloudide_plugin_.env.md#approot)
- [clipboard](cloudide_plugin_.env.md#clipboard)
- [language](cloudide_plugin_.env.md#language)
- [machineId](cloudide_plugin_.env.md#machineid)
- [sessionId](cloudide_plugin_.env.md#sessionid)
- [shell](cloudide_plugin_.env.md#shell)
- [uiKind](cloudide_plugin_.env.md#uikind)
- [uriScheme](cloudide_plugin_.env.md#urischeme)

### Functions

- [asExternalUri](cloudide_plugin_.env.md#asexternaluri)
- [getEnvVariable](cloudide_plugin_.env.md#getenvvariable)
- [getQueryParameter](cloudide_plugin_.env.md#getqueryparameter)
- [getQueryParameters](cloudide_plugin_.env.md#getqueryparameters)
- [openExternal](cloudide_plugin_.env.md#openexternal)

## Variables

### appName

• `Const` **appName**: `string`

The application name of the editor, like 'Eclipse Theia'.

#### Defined in

[index.d.ts:6412](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6412)

___

### appRoot

• `Const` **appRoot**: `string`

The application root folder from which the editor is running.

#### Defined in

[index.d.ts:6417](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6417)

___

### clipboard

• `Const` **clipboard**: [`Clipboard`](../interfaces/cloudide_plugin_.Clipboard.md)

The system clipboard.

#### Defined in

[index.d.ts:6444](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6444)

___

### language

• `Const` **language**: `string`

Represents the preferred user-language, like `de-CH`, `fr`, or `en-US`.

#### Defined in

[index.d.ts:6427](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6427)

___

### machineId

• `Const` **machineId**: `string`

A unique identifier for the computer.

#### Defined in

[index.d.ts:6449](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6449)

___

### sessionId

• `Const` **sessionId**: `string`

A unique identifier for the current session.
Changes each time the editor is started.

#### Defined in

[index.d.ts:6455](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6455)

___

### shell

• `Const` **shell**: `string`

The detected default shell for the extension host.

#### Defined in

[index.d.ts:6432](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6432)

___

### uiKind

• `Const` **uiKind**: [`UIKind`](../enums/cloudide_plugin_.UIKind.md)

The UI kind property indicates from which UI extensions
are accessed from. For example, extensions could be accessed
from a desktop application or a web browser.

#### Defined in

[index.d.ts:6439](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6439)

___

### uriScheme

• `Const` **uriScheme**: `string`

The custom uri scheme the editor registers to in the operating system.

#### Defined in

[index.d.ts:6422](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6422)

## Functions

### asExternalUri

▸ **asExternalUri**(`target`): `PromiseLike`<[`Uri`](../classes/cloudide_plugin_.Uri.md)\>

Resolves an *external* uri, such as a `http:` or `https:` link, from where the extension is running to a
uri to the same resource on the client machine.

This is a no-op if the extension is running on the client machine. Currently only supports
`https:` and `http:` uris.

If the extension is running remotely, this function automatically establishes a port forwarding tunnel
from the local machine to `target` on the remote and returns a local uri to the tunnel. The lifetime of
the port forwarding tunnel is managed by VS Code and the tunnel can be closed by the user.

Extensions should not cache the result of `asExternalUri` as the resolved uri may become invalid due to
a system or user action — for example, in remote cases, a user may close a port forwarding tunnel
that was opened by `asExternalUri`.

*Note* that uris passed through `openExternal` are automatically resolved and you should not call `asExternalUri`
on them.

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | [`Uri`](../classes/cloudide_plugin_.Uri.md) |

#### Returns

`PromiseLike`<[`Uri`](../classes/cloudide_plugin_.Uri.md)\>

A uri that can be used on the client machine.

#### Defined in

[index.d.ts:6489](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6489)

___

### getEnvVariable

▸ **getEnvVariable**(`envVarName`): `PromiseLike`<`string` \| `undefined`\>

Gets environment variable value by name.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `envVarName` | `string` | name of environment variable to get |

#### Returns

`PromiseLike`<`string` \| `undefined`\>

value of the given environment variable name or undefined if there is no such variable.

#### Defined in

[index.d.ts:6394](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6394)

___

### getQueryParameter

▸ **getQueryParameter**(`queryParamName`): `string` \| `string`[] \| `undefined`

Gets query parameter value by name.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `queryParamName` | `string` | name of query parameter to get. |

#### Returns

`string` \| `string`[] \| `undefined`

value of the given query parameter or undefined if there is no such variable.

#### Defined in

[index.d.ts:6402](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6402)

___

### getQueryParameters

▸ **getQueryParameters**(): { `[key: string]`: `string` \| `string`[];  } \| `undefined`

Returns all query parameters of current IDE.

#### Returns

{ `[key: string]`: `string` \| `string`[];  } \| `undefined`

#### Defined in

[index.d.ts:6407](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6407)

___

### openExternal

▸ **openExternal**(`target`): `PromiseLike`<`boolean`\>

Opens an *external* item, e.g. a http(s) or mailto-link, using the
default application.

*Note* that [`showTextDocument`](#window.showTextDocument) is the right
way to open a text document inside the editor, not this function.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | The uri that should be opened. |

#### Returns

`PromiseLike`<`boolean`\>

A promise indicating if open was successful.

#### Defined in

[index.d.ts:6467](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6467)
