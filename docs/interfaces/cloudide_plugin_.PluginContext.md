[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / PluginContext

# Interface: PluginContext

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).PluginContext

A plug-in context is a collection of utilities private to a
plug-in.

An instance of a `PluginContext` is provided as the first
parameter to the `start` of a plug-in.

## Table of contents

### Properties

- [environmentVariableCollection](cloudide_plugin_.PluginContext.md#environmentvariablecollection)
- [extensionMode](cloudide_plugin_.PluginContext.md#extensionmode)
- [extensionPath](cloudide_plugin_.PluginContext.md#extensionpath)
- [extensionUri](cloudide_plugin_.PluginContext.md#extensionuri)
- [globalState](cloudide_plugin_.PluginContext.md#globalstate)
- [globalStoragePath](cloudide_plugin_.PluginContext.md#globalstoragepath)
- [globalStorageUri](cloudide_plugin_.PluginContext.md#globalstorageuri)
- [logPath](cloudide_plugin_.PluginContext.md#logpath)
- [secrets](cloudide_plugin_.PluginContext.md#secrets)
- [storagePath](cloudide_plugin_.PluginContext.md#storagepath)
- [storageUri](cloudide_plugin_.PluginContext.md#storageuri)
- [subscriptions](cloudide_plugin_.PluginContext.md#subscriptions)
- [workspaceState](cloudide_plugin_.PluginContext.md#workspacestate)

### Methods

- [asAbsolutePath](cloudide_plugin_.PluginContext.md#asabsolutepath)

## Properties

### environmentVariableCollection

• `Readonly` **environmentVariableCollection**: [`EnvironmentVariableCollection`](cloudide_plugin_.EnvironmentVariableCollection.md)

Gets the extension's environment variable collection for this workspace, enabling changes
to be applied to terminal environment variables.

#### Defined in

[index.d.ts:3207](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3207)

___

### extensionMode

• `Readonly` **extensionMode**: [`ExtensionMode`](../enums/cloudide_plugin_.ExtensionMode.md)

The mode the extension is running in. This is specific to the current
extension. One extension may be in `ExtensionMode.Development` while
other extensions in the host run in `ExtensionMode.Release`.

#### Defined in

[index.d.ts:3278](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3278)

___

### extensionPath

• **extensionPath**: `string`

The absolute file path of the directory containing the extension.

#### Defined in

[index.d.ts:3196](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3196)

___

### extensionUri

• `Readonly` **extensionUri**: [`Uri`](../classes/cloudide_plugin_.Uri.md)

The uri of the directory containing the extension.

#### Defined in

[index.d.ts:3201](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3201)

___

### globalState

• **globalState**: [`Memento`](cloudide_plugin_.Memento.md) & { `setKeysForSync`: (`keys`: readonly `string`[]) => `void`  }

A memento object that stores state independent
of the current opened [workspace](#workspace.workspaceFolders).

#### Defined in

[index.d.ts:3171](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3171)

___

### globalStoragePath

• `Readonly` **globalStoragePath**: `string`

An absolute file path in which the extension can store global state.
The directory might not exist on disk and creation is
up to the extension. However, the parent directory is guaranteed to be existent.

Use [`globalState`](#PluginContext.globalState) to store key value data.

**`Deprecated`**

Use [globalStorageUri](#PluginContext.globalStorageUri) instead.

#### Defined in

[index.d.ts:3252](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3252)

___

### globalStorageUri

• `Readonly` **globalStorageUri**: [`Uri`](../classes/cloudide_plugin_.Uri.md)

The uri of a directory in which the extension can store global state.
The directory might not exist on disk and creation is
up to the extension. However, the parent directory is guaranteed to be existent.

Use [`globalState`](#PluginContext.globalState) to store key value data.

**`See`**

[`workspace.fs`](#FileSystem) for how to read and write files and folders from
 an uri.

#### Defined in

[index.d.ts:3264](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3264)

___

### logPath

• `Readonly` **logPath**: `string`

An absolute file path of a directory in which the extension can create log files.
The directory might not exist on disk and creation is up to the extension. However,
the parent directory is guaranteed to be existent.

#### Defined in

[index.d.ts:3271](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3271)

___

### secrets

• `Readonly` **secrets**: [`SecretStorage`](cloudide_plugin_.SecretStorage.md)

A storage utility for secrets.

#### Defined in

[index.d.ts:3191](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3191)

___

### storagePath

• **storagePath**: `undefined` \| `string`

An absolute file path of a workspace specific directory in which the extension
can store private state. The directory might not exist on disk and creation is
up to the extension. However, the parent directory is guaranteed to be existent.

Use [`workspaceState`](#PluginContext.workspaceState) or
[`globalState`](#PluginContext.globalState) to store key value data.

**`Deprecated`**

Use [storageUri](#PluginContext.storageUri) instead.

#### Defined in

[index.d.ts:3227](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3227)

___

### storageUri

• `Readonly` **storageUri**: `undefined` \| [`Uri`](../classes/cloudide_plugin_.Uri.md)

The uri of a workspace specific directory in which the extension
can store private state. The directory might not exist and creation is
up to the extension. However, the parent directory is guaranteed to be existent.
The value is `undefined` when no workspace nor folder has been opened.

Use [`workspaceState`](#PluginContext.workspaceState) or
[`globalState`](#PluginContext.globalState) to store key value data.

**`See`**

[`workspace.fs`](#FileSystem) for how to read and write files and folders from
 an uri.

#### Defined in

[index.d.ts:3241](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3241)

___

### subscriptions

• **subscriptions**: { `dispose`: () => `any`  }[]

An array to which disposables can be added. When this
extension is deactivated the disposables will be disposed.

#### Defined in

[index.d.ts:3159](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3159)

___

### workspaceState

• **workspaceState**: [`Memento`](cloudide_plugin_.Memento.md)

A memento object that stores state in the context
of the currently opened [workspace](#workspace.workspaceFolders).

#### Defined in

[index.d.ts:3165](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3165)

## Methods

### asAbsolutePath

▸ **asAbsolutePath**(`relativePath`): `string`

Get the absolute path of a resource contained in the extension.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `relativePath` | `string` | A relative path to a resource contained in the extension. |

#### Returns

`string`

The absolute path of the resource.

#### Defined in

[index.d.ts:3215](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3215)
