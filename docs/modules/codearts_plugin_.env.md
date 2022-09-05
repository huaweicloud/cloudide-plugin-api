[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / env

# Namespace: env

["@codearts/plugin"](_codearts_plugin_.md).env

Namespace describing the environment the editor runs in.

## Table of contents

### Variables

- [appHost](codearts_plugin_.env.md#apphost)
- [appName](codearts_plugin_.env.md#appname)
- [appRoot](codearts_plugin_.env.md#approot)
- [clipboard](codearts_plugin_.env.md#clipboard)
- [isNewAppInstall](codearts_plugin_.env.md#isnewappinstall)
- [isTelemetryEnabled](codearts_plugin_.env.md#istelemetryenabled)
- [language](codearts_plugin_.env.md#language)
- [machineId](codearts_plugin_.env.md#machineid)
- [remoteName](codearts_plugin_.env.md#remotename)
- [sessionId](codearts_plugin_.env.md#sessionid)
- [shell](codearts_plugin_.env.md#shell)
- [uiKind](codearts_plugin_.env.md#uikind)
- [uriScheme](codearts_plugin_.env.md#urischeme)

### Functions

- [asExternalUri](codearts_plugin_.env.md#asexternaluri)
- [onDidChangeTelemetryEnabled](codearts_plugin_.env.md#ondidchangetelemetryenabled)
- [openExternal](codearts_plugin_.env.md#openexternal)

## Variables

### appHost

• `Const` **appHost**: `string`

The hosted location of the application
On desktop this is 'desktop'
In the web this is the specified embedder i.e. 'github.dev', 'codespaces', or 'web' if the embedder
does not provide that information

#### Defined in

[index.d.ts:9030](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9030)

___

### appName

• `Const` **appName**: `string`

The application name of the editor, like 'VS Code'.

#### Defined in

[index.d.ts:9014](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9014)

___

### appRoot

• `Const` **appRoot**: `string`

The application root folder from which the editor is running.

*Note* that the value is the empty string when running in an
environment that has no representation of an application root folder.

#### Defined in

[index.d.ts:9022](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9022)

___

### clipboard

• `Const` **clipboard**: [`Clipboard`](../interfaces/codearts_plugin_.Clipboard.md)

The system clipboard.

#### Defined in

[index.d.ts:9045](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9045)

___

### isNewAppInstall

• `Const` **isNewAppInstall**: `boolean`

Indicates that this is a fresh install of the application.
`true` if within the first day of installation otherwise `false`.

#### Defined in

[index.d.ts:9062](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9062)

___

### isTelemetryEnabled

• `Const` **isTelemetryEnabled**: `boolean`

Indicates whether the users has telemetry enabled.
Can be observed to determine if the extension should send telemetry.

#### Defined in

[index.d.ts:9068](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9068)

___

### language

• `Const` **language**: `string`

Represents the preferred user-language, like `de-CH`, `fr`, or `en-US`.

#### Defined in

[index.d.ts:9040](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9040)

___

### machineId

• `Const` **machineId**: `string`

A unique identifier for the computer.

#### Defined in

[index.d.ts:9050](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9050)

___

### remoteName

• `Const` **remoteName**: `string` \| `undefined`

The name of a remote. Defined by extensions, popular samples are `wsl` for the Windows
Subsystem for Linux or `ssh-remote` for remotes using a secure shell.

*Note* that the value is `undefined` when there is no remote extension host but that the
value is defined in all extension hosts (local and remote) in case a remote extension host
exists. Use [extensionKind](../interfaces/codearts_plugin_.Extension.md#extensionkind) to know if
a specific extension runs remote or not.

#### Defined in

[index.d.ts:9085](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9085)

___

### sessionId

• `Const` **sessionId**: `string`

A unique identifier for the current session.
Changes each time the editor is started.

#### Defined in

[index.d.ts:9056](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9056)

___

### shell

• `Const` **shell**: `string`

The detected default shell for the extension host, this is overridden by the
`terminal.integrated.defaultProfile` setting for the extension host's platform. Note that in
environments that do not support a shell the value is the empty string.

#### Defined in

[index.d.ts:9092](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9092)

___

### uiKind

• `Const` **uiKind**: [`UIKind`](../enums/codearts_plugin_.UIKind.md)

The UI kind property indicates from which UI extensions
are accessed from. For example, extensions could be accessed
from a desktop application or a web browser.

#### Defined in

[index.d.ts:9099](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9099)

___

### uriScheme

• `Const` **uriScheme**: `string`

The custom uri scheme the editor registers to in the operating system.

#### Defined in

[index.d.ts:9035](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9035)

## Functions

### asExternalUri

▸ **asExternalUri**(`target`): [`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)\>

Resolves a uri to a form that is accessible externally.

#### `http:` or `https:` scheme

Resolves an *external* uri, such as a `http:` or `https:` link, from where the extension is running to a
uri to the same resource on the client machine.

This is a no-op if the extension is running on the client machine.

If the extension is running remotely, this function automatically establishes a port forwarding tunnel
from the local machine to `target` on the remote and returns a local uri to the tunnel. The lifetime of
the port forwarding tunnel is managed by the editor and the tunnel can be closed by the user.

*Note* that uris passed through `openExternal` are automatically resolved and you should not call `asExternalUri` on them.

#### `vscode.env.uriScheme`

Creates a uri that - if opened in a browser (e.g. via `openExternal`) - will result in a registered [UriHandler](../interfaces/codearts_plugin_.UriHandler.md)
to trigger.

Extensions should not make any assumptions about the resulting uri and should not alter it in any way.
Rather, extensions can e.g. use this uri in an authentication flow, by adding the uri as callback query
argument to the server to authenticate to.

*Note* that if the server decides to add additional query parameters to the uri (e.g. a token or secret), it
will appear in the uri that is passed to the [UriHandler](../interfaces/codearts_plugin_.UriHandler.md).

**Example** of an authentication flow:
```typescript
vscode.window.registerUriHandler({
  handleUri(uri: vscode.Uri): vscode.ProviderResult<void> {
    if (uri.path === '/did-authenticate') {
      console.log(uri.toString());
    }
  }
});

const callableUri = await vscode.env.asExternalUri(vscode.Uri.parse(vscode.env.uriScheme + '://my.extension/did-authenticate'));
await vscode.env.openExternal(callableUri);
```

*Note* that extensions should not cache the result of `asExternalUri` as the resolved uri may become invalid due to
a system or user action — for example, in remote cases, a user may close a port forwarding tunnel that was opened by
`asExternalUri`.

#### Any other scheme

Any other scheme will be handled as if the provided URI is a workspace URI. In that case, the method will return
a URI which, when handled, will make the editor open the workspace.

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | [`Uri`](../classes/codearts_plugin_.Uri.md) |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`Uri`](../classes/codearts_plugin_.Uri.md)\>

A uri that can be used on the client machine.

#### Defined in

[index.d.ts:9169](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9169)

___

### onDidChangeTelemetryEnabled

▸ **onDidChangeTelemetryEnabled**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: `boolean`) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L1603)

___

### openExternal

▸ **openExternal**(`target`): [`Thenable`](../interfaces/Thenable.md)<`boolean`\>

Opens a link externally using the default application. Depending on the
used scheme this can be:
* a browser (`http:`, `https:`)
* a mail client (`mailto:`)
* VSCode itself (`vscode:` from `vscode.env.uriScheme`)

*Note* that [`showTextDocument`](codearts_plugin_.window.md#showtextdocument) is the right
way to open a text document inside the editor, not this function.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The uri that should be opened. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`boolean`\>

A promise indicating if open was successful.

#### Defined in

[index.d.ts:9114](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9114)
