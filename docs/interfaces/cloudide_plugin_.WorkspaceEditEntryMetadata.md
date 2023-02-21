[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / WorkspaceEditEntryMetadata

# Interface: WorkspaceEditEntryMetadata

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).WorkspaceEditEntryMetadata

Additional data for entries of a workspace edit. Supports to label entries and marks entries
as needing confirmation by the user. The editor groups edits with equal labels into tree nodes,
for instance all edits labelled with "Changes in Strings" would be a tree node.

## Table of contents

### Properties

- [description](cloudide_plugin_.WorkspaceEditEntryMetadata.md#description)
- [iconPath](cloudide_plugin_.WorkspaceEditEntryMetadata.md#iconpath)
- [label](cloudide_plugin_.WorkspaceEditEntryMetadata.md#label)
- [needsConfirmation](cloudide_plugin_.WorkspaceEditEntryMetadata.md#needsconfirmation)

## Properties

### description

• `Optional` **description**: `string`

A human-readable string which is rendered less prominent on the same line.

#### Defined in

[index.d.ts:8228](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8228)

___

### iconPath

• `Optional` **iconPath**: [`Uri`](../classes/cloudide_plugin_.Uri.md) \| [`ThemeIcon`](../classes/cloudide_plugin_.ThemeIcon.md) \| { `dark`: [`Uri`](../classes/cloudide_plugin_.Uri.md) ; `light`: [`Uri`](../classes/cloudide_plugin_.Uri.md)  }

The icon path or [ThemeIcon](#ThemeIcon) for the edit.

#### Defined in

[index.d.ts:8233](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8233)

___

### label

• **label**: `string`

A human-readable string which is rendered prominent.

#### Defined in

[index.d.ts:8223](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8223)

___

### needsConfirmation

• **needsConfirmation**: `boolean`

A flag which indicates that user confirmation is needed.

#### Defined in

[index.d.ts:8218](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8218)
