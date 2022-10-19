[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WorkspaceEditEntryMetadata

# Interface: WorkspaceEditEntryMetadata

["@codearts/plugin"](../modules/_codearts_plugin_.md).WorkspaceEditEntryMetadata

Additional data for entries of a workspace edit. Supports to label entries and marks entries
as needing confirmation by the user. The editor groups edits with equal labels into tree nodes,
for instance all edits labelled with "Changes in Strings" would be a tree node.

## Table of contents

### Properties

- [description](codearts_plugin_.WorkspaceEditEntryMetadata.md#description)
- [iconPath](codearts_plugin_.WorkspaceEditEntryMetadata.md#iconpath)
- [label](codearts_plugin_.WorkspaceEditEntryMetadata.md#label)
- [needsConfirmation](codearts_plugin_.WorkspaceEditEntryMetadata.md#needsconfirmation)

## Properties

### description

• `Optional` **description**: `string`

A human-readable string which is rendered less prominent on the same line.

#### Defined in

[index.d.ts:3458](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L3458)

___

### iconPath

• `Optional` **iconPath**: [`Uri`](../classes/codearts_plugin_.Uri.md) \| [`ThemeIcon`](../classes/codearts_plugin_.ThemeIcon.md) \| { `dark`: [`Uri`](../classes/codearts_plugin_.Uri.md) ; `light`: [`Uri`](../classes/codearts_plugin_.Uri.md)  }

The icon path or [ThemeIcon](../classes/codearts_plugin_.ThemeIcon.md) for the edit.

#### Defined in

[index.d.ts:3463](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L3463)

___

### label

• **label**: `string`

A human-readable string which is rendered prominent.

#### Defined in

[index.d.ts:3453](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L3453)

___

### needsConfirmation

• **needsConfirmation**: `boolean`

A flag which indicates that user confirmation is needed.

#### Defined in

[index.d.ts:3448](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L3448)
