**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](_index_d_.md) / ["plugin"](_index_d_._plugin_.md) / env

# Namespace: env

Namespace describing the environment the editor runs in.

## Index

### Variables

* [appName](_index_d_._plugin_.env.md#appname)
* [appRoot](_index_d_._plugin_.env.md#approot)
* [clipboard](_index_d_._plugin_.env.md#clipboard)
* [language](_index_d_._plugin_.env.md#language)
* [machineId](_index_d_._plugin_.env.md#machineid)
* [remoteName](_index_d_._plugin_.env.md#remotename)
* [sessionId](_index_d_._plugin_.env.md#sessionid)
* [shell](_index_d_._plugin_.env.md#shell)
* [uiKind](_index_d_._plugin_.env.md#uikind)
* [uriScheme](_index_d_._plugin_.env.md#urischeme)

### Functions

* [asExternalUri](_index_d_._plugin_.env.md#asexternaluri)
* [openExternal](_index_d_._plugin_.env.md#openexternal)

## Variables

### appName

• `Const` **appName**: string

*Defined in [index.d.ts:7990](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7990)*

The application name of the editor, like 'VS Code'.

___

### appRoot

• `Const` **appRoot**: string

*Defined in [index.d.ts:7998](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7998)*

The application root folder from which the editor is running.

*Note* that the value is the empty string when running in an
environment that has no representation of an application root folder.

___

### clipboard

• `Const` **clipboard**: [Clipboard](../interfaces/_index_d_._plugin_.clipboard.md)

*Defined in [index.d.ts:8013](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8013)*

The system clipboard.

___

### language

• `Const` **language**: string

*Defined in [index.d.ts:8008](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8008)*

Represents the preferred user-language, like `de-CH`, `fr`, or `en-US`.

___

### machineId

• `Const` **machineId**: string

*Defined in [index.d.ts:8018](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8018)*

A unique identifier for the computer.

___

### remoteName

• `Const` **remoteName**: string \| undefined

*Defined in [index.d.ts:8035](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8035)*

The name of a remote. Defined by extensions, popular samples are `wsl` for the Windows
Subsystem for Linux or `ssh-remote` for remotes using a secure shell.

*Note* that the value is `undefined` when there is no remote extension host but that the
value is defined in all extension hosts (local and remote) in case a remote extension host
exists. Use [`Extension#extensionKind`](#Extension.extensionKind) to know if
a specific extension runs remote or not.

___

### sessionId

• `Const` **sessionId**: string

*Defined in [index.d.ts:8024](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8024)*

A unique identifier for the current session.
Changes each time the editor is started.

___

### shell

• `Const` **shell**: string

*Defined in [index.d.ts:8042](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8042)*

The detected default shell for the extension host, this is overridden by the
`terminal.integrated.shell` setting for the extension host's platform. Note that in
environments that do not support a shell the value is the empty string.

___

### uiKind

• `Const` **uiKind**: [UIKind](../enums/_index_d_._plugin_.uikind.md)

*Defined in [index.d.ts:8049](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8049)*

The UI kind property indicates from which UI extensions
are accessed from. For example, extensions could be accessed
from a desktop application or a web browser.

___

### uriScheme

• `Const` **uriScheme**: string

*Defined in [index.d.ts:8003](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8003)*

The custom uri scheme the editor registers to in the operating system.

## Functions

### asExternalUri

▸ **asExternalUri**(`target`: [Uri](../classes/_index_d_._plugin_.uri.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<[Uri](../classes/_index_d_._plugin_.uri.md)>

*Defined in [index.d.ts:8115](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8115)*

Resolves a uri to form that is accessible externally. Currently only supports `https:`, `http:` and
`vscode.env.uriScheme` uris.

#### `http:` or `https:` scheme

Resolves an *external* uri, such as a `http:` or `https:` link, from where the extension is running to a
uri to the same resource on the client machine.

This is a no-op if the extension is running on the client machine.

If the extension is running remotely, this function automatically establishes a port forwarding tunnel
from the local machine to `target` on the remote and returns a local uri to the tunnel. The lifetime of
the port forwarding tunnel is managed by VS Code and the tunnel can be closed by the user.

*Note* that uris passed through `openExternal` are automatically resolved and you should not call `asExternalUri` on them.

#### `vscode.env.uriScheme`

Creates a uri that - if opened in a browser (e.g. via `openExternal`) - will result in a registered [UriHandler](#UriHandler)
to trigger.

Extensions should not make any assumptions about the resulting uri and should not alter it in anyway.
Rather, extensions can e.g. use this uri in an authentication flow, by adding the uri as callback query
argument to the server to authenticate to.

*Note* that if the server decides to add additional query parameters to the uri (e.g. a token or secret), it
will appear in the uri that is passed to the [UriHandler](#UriHandler).

**Example** of an authentication flow:
```typescript
vscode.window.registerUriHandler({
  handleUri(uri: vscode.Uri): vscode.ProviderResult<void> {
    if (uri.path === '/did-authenticate') {
      console.log(uri.toString());
    }
  }
});

const callableUri = await vscode.env.asExternalUri(vscode.Uri.parse(`${vscode.env.uriScheme}://my.extension/did-authenticate`));
await vscode.env.openExternal(callableUri);
```

*Note* that extensions should not cache the result of `asExternalUri` as the resolved uri may become invalid due to
a system or user action — for example, in remote cases, a user may close a port forwarding tunnel that was opened by
`asExternalUri`.

#### Parameters:

Name | Type |
------ | ------ |
`target` | [Uri](../classes/_index_d_._plugin_.uri.md) |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[Uri](../classes/_index_d_._plugin_.uri.md)>

A uri that can be used on the client machine.

___

### openExternal

▸ **openExternal**(`target`: [Uri](../classes/_index_d_._plugin_.uri.md)): [Thenable](../interfaces/_index_d_.thenable.md)\<boolean>

*Defined in [index.d.ts:8064](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L8064)*

Opens a link externally using the default application. Depending on the
used scheme this can be:
* a browser (`http:`, `https:`)
* a mail client (`mailto:`)
* VSCode itself (`vscode:` from `vscode.env.uriScheme`)

*Note* that [`showTextDocument`](#window.showTextDocument) is the right
way to open a text document inside the editor, not this function.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`target` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri that should be opened. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<boolean>

A promise indicating if open was successful.
