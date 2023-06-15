[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ExtensionContext

# Interface: ExtensionContext

["@codearts/plugin"](../modules/_codearts_plugin_.md).ExtensionContext

An extension context is a collection of utilities private to an
extension.

An instance of an `ExtensionContext` is provided as the first
parameter to the `activate`-call of an extension.

## Table of contents

### Properties

- [environmentVariableCollection](codearts_plugin_.ExtensionContext.md#environmentvariablecollection)
- [extension](codearts_plugin_.ExtensionContext.md#extension)
- [extensionMode](codearts_plugin_.ExtensionContext.md#extensionmode)
- [extensionPath](codearts_plugin_.ExtensionContext.md#extensionpath)
- [extensionUri](codearts_plugin_.ExtensionContext.md#extensionuri)
- [globalState](codearts_plugin_.ExtensionContext.md#globalstate)
- [globalStoragePath](codearts_plugin_.ExtensionContext.md#globalstoragepath)
- [globalStorageUri](codearts_plugin_.ExtensionContext.md#globalstorageuri)
- [logPath](codearts_plugin_.ExtensionContext.md#logpath)
- [logUri](codearts_plugin_.ExtensionContext.md#loguri)
- [secrets](codearts_plugin_.ExtensionContext.md#secrets)
- [storagePath](codearts_plugin_.ExtensionContext.md#storagepath)
- [storageUri](codearts_plugin_.ExtensionContext.md#storageuri)
- [subscriptions](codearts_plugin_.ExtensionContext.md#subscriptions)
- [workspaceState](codearts_plugin_.ExtensionContext.md#workspacestate)

### Methods

- [asAbsolutePath](codearts_plugin_.ExtensionContext.md#asabsolutepath)

## Properties

### environmentVariableCollection

• `Readonly` **environmentVariableCollection**: [`EnvironmentVariableCollection`](codearts_plugin_.EnvironmentVariableCollection.md)

Gets the extension's environment variable collection for this workspace, enabling changes
to be applied to terminal environment variables.

#### Defined in

[index.d.ts:6938](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L6938)

___

### extension

• `Readonly` **extension**: [`Extension`](codearts_plugin_.Extension.md)<`any`\>

The current `Extension` instance.

#### Defined in

[index.d.ts:7029](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L7029)

___

### extensionMode

• `Readonly` **extensionMode**: [`ExtensionMode`](../enums/codearts_plugin_.ExtensionMode.md)

The mode the extension is running in. This is specific to the current
extension. One extension may be in `ExtensionMode.Development` while
other extensions in the host run in `ExtensionMode.Release`.

#### Defined in

[index.d.ts:7024](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L7024)

___

### extensionPath

• `Readonly` **extensionPath**: `string`

The absolute file path of the directory containing the extension. Shorthand
notation for [ExtensionContext.extensionUri.fsPath](codearts_plugin_.TextDocument.md#uri) (independent of the uri scheme).

#### Defined in

[index.d.ts:6932](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L6932)

___

### extensionUri

• `Readonly` **extensionUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The uri of the directory containing the extension.

#### Defined in

[index.d.ts:6926](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L6926)

___

### globalState

• `Readonly` **globalState**: [`Memento`](codearts_plugin_.Memento.md) & { `setKeysForSync`: (`keys`: readonly `string`[]) => `void`  }

A memento object that stores state independent
of the current opened [workspace](../modules/codearts_plugin_.workspace.md#workspacefolders).

#### Defined in

[index.d.ts:6900](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L6900)

___

### globalStoragePath

• `Readonly` **globalStoragePath**: `string`

An absolute file path in which the extension can store global state.
The directory might not exist on disk and creation is
up to the extension. However, the parent directory is guaranteed to be existent.

Use [`globalState`](codearts_plugin_.ExtensionContext.md#globalstate) to store key value data.

**`Deprecated`**

Use [globalStorageUri](codearts_plugin_.ExtensionContext.md#globalstorageuri) instead.

#### Defined in

[index.d.ts:6998](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L6998)

___

### globalStorageUri

• `Readonly` **globalStorageUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The uri of a directory in which the extension can store global state.
The directory might not exist on disk and creation is
up to the extension. However, the parent directory is guaranteed to be existent.

Use [`globalState`](codearts_plugin_.ExtensionContext.md#globalstate) to store key value data.

**`See`**

[`workspace.fs`](codearts_plugin_.FileSystem.md) for how to read and write files and folders from
 an uri.

#### Defined in

[index.d.ts:6987](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L6987)

___

### logPath

• `Readonly` **logPath**: `string`

An absolute file path of a directory in which the extension can create log files.
The directory might not exist on disk and creation is up to the extension. However,
the parent directory is guaranteed to be existent.

**`Deprecated`**

Use [logUri](codearts_plugin_.ExtensionContext.md#loguri) instead.

#### Defined in

[index.d.ts:7017](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L7017)

___

### logUri

• `Readonly` **logUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The uri of a directory in which the extension can create log files.
The directory might not exist on disk and creation is up to the extension. However,
the parent directory is guaranteed to be existent.

**`See`**

[`workspace.fs`](codearts_plugin_.FileSystem.md) for how to read and write files and folders from
 an uri.

#### Defined in

[index.d.ts:7008](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L7008)

___

### secrets

• `Readonly` **secrets**: [`SecretStorage`](codearts_plugin_.SecretStorage.md)

A storage utility for secrets. Secrets are persisted across reloads and are independent of the
current opened [workspace](../modules/codearts_plugin_.workspace.md#workspacefolders).

#### Defined in

[index.d.ts:6921](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L6921)

___

### storagePath

• `Readonly` **storagePath**: `undefined` \| `string`

An absolute file path of a workspace specific directory in which the extension
can store private state. The directory might not exist on disk and creation is
up to the extension. However, the parent directory is guaranteed to be existent.

Use [`workspaceState`](codearts_plugin_.ExtensionContext.md#workspacestate) or
[`globalState`](codearts_plugin_.ExtensionContext.md#globalstate) to store key value data.

**`Deprecated`**

Use [storageUri](codearts_plugin_.ExtensionContext.md#storageuri) instead.

#### Defined in

[index.d.ts:6975](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L6975)

___

### storageUri

• `Readonly` **storageUri**: `undefined` \| [`Uri`](../classes/codearts_plugin_.Uri.md)

The uri of a workspace specific directory in which the extension
can store private state. The directory might not exist and creation is
up to the extension. However, the parent directory is guaranteed to be existent.
The value is `undefined` when no workspace nor folder has been opened.

Use [`workspaceState`](codearts_plugin_.ExtensionContext.md#workspacestate) or
[`globalState`](codearts_plugin_.ExtensionContext.md#globalstate) to store key value data.

**`See`**

[`workspace.fs`](codearts_plugin_.FileSystem.md) for how to read and write files and folders from
 an uri.

#### Defined in

[index.d.ts:6963](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L6963)

___

### subscriptions

• `Readonly` **subscriptions**: { `dispose`: () => `any`  }[]

An array to which disposables can be added. When this
extension is deactivated the disposables will be disposed.

*Note* that asynchronous dispose-functions aren't awaited.

#### Defined in

[index.d.ts:6888](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L6888)

___

### workspaceState

• `Readonly` **workspaceState**: [`Memento`](codearts_plugin_.Memento.md)

A memento object that stores state in the context
of the currently opened [workspace](../modules/codearts_plugin_.workspace.md#workspacefolders).

#### Defined in

[index.d.ts:6894](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L6894)

## Methods

### asAbsolutePath

▸ **asAbsolutePath**(`relativePath`): `string`

Get the absolute path of a resource contained in the extension.

*Note* that an absolute uri can be constructed via [`joinPath`](../classes/codearts_plugin_.Uri.md#joinpath) and
[`extensionUri`](codearts_plugin_.ExtensionContext.md#extensionuri), e.g. `vscode.Uri.joinPath(context.extensionUri, relativePath);`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `relativePath` | `string` | A relative path to a resource contained in the extension. |

#### Returns

`string`

The absolute path of the resource.

#### Defined in

[index.d.ts:6949](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L6949)
