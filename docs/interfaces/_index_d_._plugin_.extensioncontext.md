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

* [extensionPath](_index_d_._plugin_.extensioncontext.md#extensionpath)
* [extensionUri](_index_d_._plugin_.extensioncontext.md#extensionuri)
* [globalState](_index_d_._plugin_.extensioncontext.md#globalstate)
* [globalStoragePath](_index_d_._plugin_.extensioncontext.md#globalstoragepath)
* [logPath](_index_d_._plugin_.extensioncontext.md#logpath)
* [storagePath](_index_d_._plugin_.extensioncontext.md#storagepath)
* [subscriptions](_index_d_._plugin_.extensioncontext.md#subscriptions)
* [workspaceState](_index_d_._plugin_.extensioncontext.md#workspacestate)

### Methods

* [asAbsolutePath](_index_d_._plugin_.extensioncontext.md#asabsolutepath)

## Properties

### extensionPath

• `Readonly` **extensionPath**: string

*Defined in [index.d.ts:5461](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5461)*

The absolute file path of the directory containing the extension. Shorthand
notation for [ExtensionContext.extensionUri.fsPath](#TextDocument.uri) (independent of the uri scheme).

___

### extensionUri

• `Readonly` **extensionUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:5455](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5455)*

The uri of the directory containing the extension.

___

### globalState

• `Readonly` **globalState**: [Memento](_index_d_._plugin_.memento.md)

*Defined in [index.d.ts:5450](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5450)*

A memento object that stores state independent
of the current opened [workspace](#workspace.workspaceFolders).

___

### globalStoragePath

• `Readonly` **globalStoragePath**: string

*Defined in [index.d.ts:5488](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5488)*

An absolute file path in which the extension can store global state.
The directory might not exist on disk and creation is
up to the extension. However, the parent directory is guaranteed to be existent.

Use [`globalState`](#ExtensionContext.globalState) to store key value data.

___

### logPath

• `Readonly` **logPath**: string

*Defined in [index.d.ts:5495](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5495)*

An absolute file path of a directory in which the extension can create log files.
The directory might not exist on disk and creation is up to the extension. However,
the parent directory is guaranteed to be existent.

___

### storagePath

• `Readonly` **storagePath**: string \| undefined

*Defined in [index.d.ts:5479](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5479)*

An absolute file path of a workspace specific directory in which the extension
can store private state. The directory might not exist on disk and creation is
up to the extension. However, the parent directory is guaranteed to be existent.

Use [`workspaceState`](#ExtensionContext.workspaceState) or
[`globalState`](#ExtensionContext.globalState) to store key value data.

___

### subscriptions

• `Readonly` **subscriptions**: { dispose: () => any  }[]

*Defined in [index.d.ts:5438](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5438)*

An array to which disposables can be added. When this
extension is deactivated the disposables will be disposed.

___

### workspaceState

• `Readonly` **workspaceState**: [Memento](_index_d_._plugin_.memento.md)

*Defined in [index.d.ts:5444](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5444)*

A memento object that stores state in the context
of the currently opened [workspace](#workspace.workspaceFolders).

## Methods

### asAbsolutePath

▸ **asAbsolutePath**(`relativePath`: string): string

*Defined in [index.d.ts:5469](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5469)*

Get the absolute path of a resource contained in the extension.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`relativePath` | string | A relative path to a resource contained in the extension. |

**Returns:** string

The absolute path of the resource.
