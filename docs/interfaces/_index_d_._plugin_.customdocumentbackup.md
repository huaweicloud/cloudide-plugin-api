**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CustomDocumentBackup

# Interface: CustomDocumentBackup

A backup for an [`CustomDocument`](#CustomDocument).

## Hierarchy

* **CustomDocumentBackup**

## Index

### Properties

* [id](_index_d_._plugin_.customdocumentbackup.md#id)

### Methods

* [delete](_index_d_._plugin_.customdocumentbackup.md#delete)

## Properties

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:7750](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7750)*

Unique identifier for the backup.

This id is passed back to your extension in `openCustomDocument` when opening a custom editor from a backup.

## Methods

### delete

▸ **delete**(): void

*Defined in [index.d.ts:7758](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7758)*

Delete the current backup.

This is called by VS Code when it is clear the current backup is no longer needed, such as when a new backup
is made or when the file is saved.

**Returns:** void
