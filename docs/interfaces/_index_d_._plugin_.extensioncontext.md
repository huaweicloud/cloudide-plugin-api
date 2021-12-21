**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ExtensionContext

# Interface: ExtensionContext

An extension context is a collection of utilities private to an
extension.

An instance of an `ExtensionContext` is provided as the first
parameter to the `activate`-call of an extension.

## Hierarchy

* **ExtensionContext**

## Index

### Properties

* [environmentVariableCollection](_index_d_._plugin_.extensioncontext.md#environmentvariablecollection)
* [extensionMode](_index_d_._plugin_.extensioncontext.md#extensionmode)
* [extensionPath](_index_d_._plugin_.extensioncontext.md#extensionpath)
* [extensionUri](_index_d_._plugin_.extensioncontext.md#extensionuri)
* [globalState](_index_d_._plugin_.extensioncontext.md#globalstate)
* [globalStoragePath](_index_d_._plugin_.extensioncontext.md#globalstoragepath)
* [globalStorageUri](_index_d_._plugin_.extensioncontext.md#globalstorageuri)
* [logPath](_index_d_._plugin_.extensioncontext.md#logpath)
* [logUri](_index_d_._plugin_.extensioncontext.md#loguri)
* [secrets](_index_d_._plugin_.extensioncontext.md#secrets)
* [storagePath](_index_d_._plugin_.extensioncontext.md#storagepath)
* [storageUri](_index_d_._plugin_.extensioncontext.md#storageuri)
* [subscriptions](_index_d_._plugin_.extensioncontext.md#subscriptions)
* [workspaceState](_index_d_._plugin_.extensioncontext.md#workspacestate)

### Methods

* [asAbsolutePath](_index_d_._plugin_.extensioncontext.md#asabsolutepath)

## Properties

### environmentVariableCollection

• `Readonly` **environmentVariableCollection**: [EnvironmentVariableCollection](_index_d_._plugin_.environmentvariablecollection.md)

*Defined in [index.d.ts:5966](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5966)*

Gets the extension's environment variable collection for this workspace, enabling changes
to be applied to terminal environment variables.

___

### extensionMode

• `Readonly` **extensionMode**: [ExtensionMode](../enums/_index_d_._plugin_.extensionmode.md)

*Defined in [index.d.ts:6052](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6052)*

The mode the extension is running in. This is specific to the current
extension. One extension may be in `ExtensionMode.Development` while
other extensions in the host run in `ExtensionMode.Release`.

___

### extensionPath

• `Readonly` **extensionPath**: string

*Defined in [index.d.ts:5960](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5960)*

The absolute file path of the directory containing the extension. Shorthand
notation for [ExtensionContext.extensionUri.fsPath](#TextDocument.uri) (independent of the uri scheme).

___

### extensionUri

• `Readonly` **extensionUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:5954](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5954)*

The uri of the directory containing the extension.

___

### globalState

• `Readonly` **globalState**: [Memento](_index_d_._plugin_.memento.md) & { setKeysForSync: (keys: string[]) => void  }

*Defined in [index.d.ts:5929](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5929)*

A memento object that stores state independent
of the current opened [workspace](#workspace.workspaceFolders).

___

### globalStoragePath

• `Readonly` **globalStoragePath**: string

*Defined in [index.d.ts:6026](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6026)*

An absolute file path in which the extension can store global state.
The directory might not exist on disk and creation is
up to the extension. However, the parent directory is guaranteed to be existent.

Use [`globalState`](#ExtensionContext.globalState) to store key value data.

**`deprecated`** Use [globalStorageUri](#ExtensionContext.globalStorageUri) instead.

___

### globalStorageUri

• `Readonly` **globalStorageUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:6015](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6015)*

The uri of a directory in which the extension can store global state.
The directory might not exist on disk and creation is
up to the extension. However, the parent directory is guaranteed to be existent.

Use [`globalState`](#ExtensionContext.globalState) to store key value data.

**`see`** [`workspace.fs`](#FileSystem) for how to read and write files and folders from
 an uri.

___

### logPath

• `Readonly` **logPath**: string

*Defined in [index.d.ts:6045](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6045)*

An absolute file path of a directory in which the extension can create log files.
The directory might not exist on disk and creation is up to the extension. However,
the parent directory is guaranteed to be existent.

**`deprecated`** Use [logUri](#ExtensionContext.logUri) instead.

___

### logUri

• `Readonly` **logUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:6036](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6036)*

The uri of a directory in which the extension can create log files.
The directory might not exist on disk and creation is up to the extension. However,
the parent directory is guaranteed to be existent.

**`see`** [`workspace.fs`](#FileSystem) for how to read and write files and folders from
 an uri.

___

### secrets

• `Readonly` **secrets**: [SecretStorage](_index_d_._plugin_.secretstorage.md)

*Defined in [index.d.ts:5949](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5949)*

A storage utility for secrets.

___

### storagePath

• `Readonly` **storagePath**: string \| undefined

*Defined in [index.d.ts:6003](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6003)*

An absolute file path of a workspace specific directory in which the extension
can store private state. The directory might not exist on disk and creation is
up to the extension. However, the parent directory is guaranteed to be existent.

Use [`workspaceState`](#ExtensionContext.workspaceState) or
[`globalState`](#ExtensionContext.globalState) to store key value data.

**`deprecated`** Use [storageUri](#ExtensionContext.storageUri) instead.

___

### storageUri

• `Readonly` **storageUri**: [Uri](../classes/_index_d_._plugin_.uri.md) \| undefined

*Defined in [index.d.ts:5991](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5991)*

The uri of a workspace specific directory in which the extension
can store private state. The directory might not exist and creation is
up to the extension. However, the parent directory is guaranteed to be existent.
The value is `undefined` when no workspace nor folder has been opened.

Use [`workspaceState`](#ExtensionContext.workspaceState) or
[`globalState`](#ExtensionContext.globalState) to store key value data.

**`see`** [`workspace.fs`](#FileSystem) for how to read and write files and folders from
 an uri.

___

### subscriptions

• `Readonly` **subscriptions**: { dispose: () => any  }[]

*Defined in [index.d.ts:5917](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5917)*

An array to which disposables can be added. When this
extension is deactivated the disposables will be disposed.

___

### workspaceState

• `Readonly` **workspaceState**: [Memento](_index_d_._plugin_.memento.md)

*Defined in [index.d.ts:5923](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5923)*

A memento object that stores state in the context
of the currently opened [workspace](#workspace.workspaceFolders).

## Methods

### asAbsolutePath

▸ **asAbsolutePath**(`relativePath`: string): string

*Defined in [index.d.ts:5977](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5977)*

Get the absolute path of a resource contained in the extension.

*Note* that an absolute uri can be constructed via [`Uri.joinPath`](#Uri.joinPath) and
[`extensionUri`](#ExtensionContext.extensionUri), e.g. `vscode.Uri.joinPath(context.extensionUri, relativePath);`

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`relativePath` | string | A relative path to a resource contained in the extension. |

**Returns:** string

The absolute path of the resource.
