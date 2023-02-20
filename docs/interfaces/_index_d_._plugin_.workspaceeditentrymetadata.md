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

*Defined in [index.d.ts:3192](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L3192)*

A human-readable string which is rendered less prominent on the same line.

___

### iconPath

• `Optional` **iconPath**: [Uri](../classes/_index_d_._plugin_.uri.md) \| { dark: [Uri](../classes/_index_d_._plugin_.uri.md) ; light: [Uri](../classes/_index_d_._plugin_.uri.md)  } \| [ThemeIcon](../classes/_index_d_._plugin_.themeicon.md)

*Defined in [index.d.ts:3197](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L3197)*

The icon path or [ThemeIcon](#ThemeIcon) for the edit.

___

### label

•  **label**: string

*Defined in [index.d.ts:3187](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L3187)*

A human-readable string which is rendered prominent.

___

### needsConfirmation

•  **needsConfirmation**: boolean

*Defined in [index.d.ts:3182](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L3182)*

A flag which indicates that user confirmation is needed.
