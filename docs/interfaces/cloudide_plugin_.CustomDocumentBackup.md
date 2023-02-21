[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CustomDocumentBackup

# Interface: CustomDocumentBackup

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CustomDocumentBackup

A backup for an [`CustomDocument`](#CustomDocument).

## Table of contents

### Properties

- [id](cloudide_plugin_.CustomDocumentBackup.md#id)

### Methods

- [delete](cloudide_plugin_.CustomDocumentBackup.md#delete)

## Properties

### id

• `Readonly` **id**: `string`

Unique identifier for the backup.

This id is passed back to your extension in `openCustomDocument` when opening a custom editor from a backup.

#### Defined in

[index.d.ts:3906](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3906)

## Methods

### delete

▸ **delete**(): `void`

Delete the current backup.

This is called by VS Code when it is clear the current backup is no longer needed, such as when a new backup
is made or when the file is saved.

#### Returns

`void`

#### Defined in

[index.d.ts:3914](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3914)
