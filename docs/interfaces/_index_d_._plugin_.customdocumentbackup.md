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

*Defined in [index.d.ts:7747](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7747)*

Unique identifier for the backup.

This id is passed back to your extension in `openCustomDocument` when opening a custom editor from a backup.

## Methods

### delete

▸ **delete**(): void

*Defined in [index.d.ts:7755](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L7755)*

Delete the current backup.

This is called by VS Code when it is clear the current backup is no longer needed, such as when a new backup
is made or when the file is saved.

**Returns:** void
