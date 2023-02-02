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

[index.d.ts:6903](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6903)

___

### extension

• `Readonly` **extension**: [`Extension`](codearts_plugin_.Extension.md)<`any`\>

The current `Extension` instance.

#### Defined in

[index.d.ts:6994](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6994)

___

### extensionMode

• `Readonly` **extensionMode**: [`ExtensionMode`](../enums/codearts_plugin_.ExtensionMode.md)

The mode the extension is running in. This is specific to the current
extension. One extension may be in `ExtensionMode.Development` while
other extensions in the host run in `ExtensionMode.Release`.

#### Defined in

[index.d.ts:6989](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6989)

___

### extensionPath

• `Readonly` **extensionPath**: `string`

The absolute file path of the directory containing the extension. Shorthand
notation for [ExtensionContext.extensionUri.fsPath](codearts_plugin_.TextDocument.md#uri) (independent of the uri scheme).

#### Defined in

[index.d.ts:6897](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6897)

___

### extensionUri

• `Readonly` **extensionUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The uri of the directory containing the extension.

#### Defined in

[index.d.ts:6891](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6891)

___

### globalState

• `Readonly` **globalState**: [`Memento`](codearts_plugin_.Memento.md) & { `setKeysForSync`: (`keys`: readonly `string`[]) => `void`  }

A memento object that stores state independent
of the current opened [workspace](../modules/codearts_plugin_.workspace.md#workspacefolders).

#### Defined in

[index.d.ts:6865](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6865)

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

[index.d.ts:6963](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6963)

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

[index.d.ts:6952](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6952)

___

### logPath

• `Readonly` **logPath**: `string`

An absolute file path of a directory in which the extension can create log files.
The directory might not exist on disk and creation is up to the extension. However,
the parent directory is guaranteed to be existent.

**`Deprecated`**

Use [logUri](codearts_plugin_.ExtensionContext.md#loguri) instead.

#### Defined in

[index.d.ts:6982](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6982)

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

[index.d.ts:6973](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6973)

___

### secrets

• `Readonly` **secrets**: [`SecretStorage`](codearts_plugin_.SecretStorage.md)

A storage utility for secrets. Secrets are persisted across reloads and are independent of the
current opened [workspace](../modules/codearts_plugin_.workspace.md#workspacefolders).

#### Defined in

[index.d.ts:6886](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6886)

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

[index.d.ts:6940](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6940)

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

[index.d.ts:6928](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6928)

___

### subscriptions

• `Readonly` **subscriptions**: { `dispose`: () => `any`  }[]

An array to which disposables can be added. When this
extension is deactivated the disposables will be disposed.

*Note* that asynchronous dispose-functions aren't awaited.

#### Defined in

[index.d.ts:6853](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6853)

___

### workspaceState

• `Readonly` **workspaceState**: [`Memento`](codearts_plugin_.Memento.md)

A memento object that stores state in the context
of the currently opened [workspace](../modules/codearts_plugin_.workspace.md#workspacefolders).

#### Defined in

[index.d.ts:6859](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6859)

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

[index.d.ts:6914](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6914)
