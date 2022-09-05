[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WorkspaceFolder

# Interface: WorkspaceFolder

["@codearts/plugin"](../modules/_codearts_plugin_.md).WorkspaceFolder

A workspace folder is one of potentially many roots opened by the editor. All workspace folders
are equal which means there is no notion of an active or primary workspace folder.

## Table of contents

### Properties

- [index](codearts_plugin_.WorkspaceFolder.md#index)
- [name](codearts_plugin_.WorkspaceFolder.md#name)
- [uri](codearts_plugin_.WorkspaceFolder.md#uri)

## Properties

### index

• `Readonly` **index**: `number`

The ordinal number of this workspace folder.

#### Defined in

[index.d.ts:11627](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11627)

___

### name

• `Readonly` **name**: `string`

The name of this workspace folder. Defaults to
the basename of its [uri-path](../classes/codearts_plugin_.Uri.md#path)

#### Defined in

[index.d.ts:11622](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11622)

___

### uri

• `Readonly` **uri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The associated uri for this workspace folder.

*Note:* The [Uri](../classes/codearts_plugin_.Uri.md)-type was intentionally chosen such that future releases of the editor can support
workspace folders that are not stored on the local disk, e.g. `ftp://server/workspaces/foo`.

#### Defined in

[index.d.ts:11616](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11616)
