**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / WorkspaceEditEntryMetadata

# Interface: WorkspaceEditEntryMetadata

Additional data for entries of a workspace edit. Supports to label entries and marks entries
as needing confirmation by the user. The editor groups edits with equal labels into tree nodes,
for instance all edits labelled with "Changes in Strings" would be a tree node.

## Hierarchy

* **WorkspaceEditEntryMetadata**

## Index

### Properties

* [description](_index_d_._plugin_.workspaceeditentrymetadata.md#description)
* [iconPath](_index_d_._plugin_.workspaceeditentrymetadata.md#iconpath)
* [label](_index_d_._plugin_.workspaceeditentrymetadata.md#label)
* [needsConfirmation](_index_d_._plugin_.workspaceeditentrymetadata.md#needsconfirmation)

## Properties

### description

• `Optional` **description**: string

*Defined in [index.d.ts:2963](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2963)*

A human-readable string which is rendered less prominent on the same line.

___

### iconPath

• `Optional` **iconPath**: [Uri](../classes/_index_d_._plugin_.uri.md) \| { dark: [Uri](../classes/_index_d_._plugin_.uri.md) ; light: [Uri](../classes/_index_d_._plugin_.uri.md)  } \| [ThemeIcon](../classes/_index_d_._plugin_.themeicon.md)

*Defined in [index.d.ts:2968](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2968)*

The icon path or [ThemeIcon](#ThemeIcon) for the edit.

___

### label

•  **label**: string

*Defined in [index.d.ts:2958](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2958)*

A human-readable string which is rendered prominent.

___

### needsConfirmation

•  **needsConfirmation**: boolean

*Defined in [index.d.ts:2953](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2953)*

A flag which indicates that user confirmation is needed.
