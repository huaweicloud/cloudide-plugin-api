**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / WorkspaceFolder

# Interface: WorkspaceFolder

A workspace folder is one of potentially many roots opened by the editor. All workspace folders
are equal which means there is no notion of an active or primary workspace folder.

## Hierarchy

* **WorkspaceFolder**

## Index

### Properties

* [index](_index_d_._plugin_.workspacefolder.md#index)
* [name](_index_d_._plugin_.workspacefolder.md#name)
* [uri](_index_d_._plugin_.workspacefolder.md#uri)

## Properties

### index

• `Readonly` **index**: number

*Defined in [index.d.ts:10315](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L10315)*

The ordinal number of this workspace folder.

___

### name

• `Readonly` **name**: string

*Defined in [index.d.ts:10310](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L10310)*

The name of this workspace folder. Defaults to
the basename of its [uri-path](#Uri.path)

___

### uri

• `Readonly` **uri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:10304](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L10304)*

The associated uri for this workspace folder.

*Note:* The [Uri](#Uri)-type was intentionally chosen such that future releases of the editor can support
workspace folders that are not stored on the local disk, e.g. `ftp://server/workspaces/foo`.
