[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / WorkspaceFolder

# Interface: WorkspaceFolder

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).WorkspaceFolder

A workspace folder is one of potentially many roots opened by the editor. All workspace folders
are equal which means there is no notion of an active or master workspace folder.

## Table of contents

### Properties

- [index](cloudide_plugin_.WorkspaceFolder.md#index)
- [name](cloudide_plugin_.WorkspaceFolder.md#name)
- [uri](cloudide_plugin_.WorkspaceFolder.md#uri)

## Properties

### index

• `Readonly` **index**: `number`

The ordinal number of this workspace folder.

#### Defined in

[index.d.ts:5591](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5591)

___

### name

• `Readonly` **name**: `string`

The name of this workspace folder. Defaults to
the basename of its [uri-path](#Uri.path)

#### Defined in

[index.d.ts:5586](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5586)

___

### uri

• `Readonly` **uri**: [`Uri`](../classes/cloudide_plugin_.Uri.md)

The associated uri for this workspace folder.

*Note:* The [Uri](#Uri)-type was intentionally chosen such that future releases of the editor can support
workspace folders that are not stored on the local disk, e.g. `ftp://server/workspaces/foo`.

#### Defined in

[index.d.ts:5580](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5580)
