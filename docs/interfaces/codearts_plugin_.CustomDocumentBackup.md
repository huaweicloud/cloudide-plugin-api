[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CustomDocumentBackup

# Interface: CustomDocumentBackup

["@codearts/plugin"](../modules/_codearts_plugin_.md).CustomDocumentBackup

A backup for an [`CustomDocument`](codearts_plugin_.CustomDocument.md).

## Table of contents

### Properties

- [id](codearts_plugin_.CustomDocumentBackup.md#id)

### Methods

- [delete](codearts_plugin_.CustomDocumentBackup.md#delete)

## Properties

### id

• `Readonly` **id**: `string`

Unique identifier for the backup.

This id is passed back to your extension in `openCustomDocument` when opening a custom editor from a backup.

#### Defined in

[index.d.ts:8865](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8865)

## Methods

### delete

▸ **delete**(): `void`

Delete the current backup.

This is called by the editor when it is clear the current backup is no longer needed, such as when a new backup
is made or when the file is saved.

#### Returns

`void`

#### Defined in

[index.d.ts:8873](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8873)
