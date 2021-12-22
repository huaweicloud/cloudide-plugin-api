**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CustomDocumentBackupContext

# Interface: CustomDocumentBackupContext

Additional information used to implement [`CustomEditableDocument.backup`](#CustomEditableDocument.backup).

## Hierarchy

* **CustomDocumentBackupContext**

## Index

### Properties

* [destination](_index_d_._plugin_.customdocumentbackupcontext.md#destination)

## Properties

### destination

• `Readonly` **destination**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:7774](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L7774)*

Suggested file location to write the new backup.

Note that your extension is free to ignore this and use its own strategy for backup.

If the editor is for a resource from the current workspace, `destination` will point to a file inside
`ExtensionContext.storagePath`. The parent folder of `destination` may not exist, so make sure to created it
before writing the backup to this location.
