[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WorkspaceFolderPickOptions

# Interface: WorkspaceFolderPickOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).WorkspaceFolderPickOptions

Options to configure the behaviour of the [workspace folder](codearts_plugin_.WorkspaceFolder.md) pick UI.

## Table of contents

### Properties

- [ignoreFocusOut](codearts_plugin_.WorkspaceFolderPickOptions.md#ignorefocusout)
- [placeHolder](codearts_plugin_.WorkspaceFolderPickOptions.md#placeholder)

## Properties

### ignoreFocusOut

• `Optional` **ignoreFocusOut**: `boolean`

Set to `true` to keep the picker open when focus moves to another part of the editor or to another window.
This setting is ignored on iPad and is always false.

#### Defined in

[index.d.ts:1847](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L1847)

___

### placeHolder

• `Optional` **placeHolder**: `string`

An optional string to show as placeholder in the input box to guide the user what to pick on.

#### Defined in

[index.d.ts:1841](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L1841)
