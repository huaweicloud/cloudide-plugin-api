**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CustomDocumentOpenContext

# Interface: CustomDocumentOpenContext

Additional information about the opening custom document.

## Hierarchy

* **CustomDocumentOpenContext**

## Index

### Properties

* [backupId](_index_d_._plugin_.customdocumentopencontext.md#backupid)

## Properties

### backupId

• `Optional` `Readonly` **backupId**: string

*Defined in [index.d.ts:7787](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7787)*

The id of the backup to restore the document from or `undefined` if there is no backup.

If this is provided, your extension should restore the editor from the backup instead of reading the file
from the user's workspace.
