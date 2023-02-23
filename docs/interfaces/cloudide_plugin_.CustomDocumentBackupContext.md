[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CustomDocumentBackupContext

# Interface: CustomDocumentBackupContext

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CustomDocumentBackupContext

Additional information used to implement [`CustomEditableDocument.backup`](#CustomEditableDocument.backup).

## Table of contents

### Properties

- [destination](cloudide_plugin_.CustomDocumentBackupContext.md#destination)

## Properties

### destination

• `Readonly` **destination**: [`Uri`](../classes/cloudide_plugin_.Uri.md)

Suggested file location to write the new backup.

Note that your extension is free to ignore this and use its own strategy for backup.

If the editor is for a resource from the current workspace, `destination` will point to a file inside
`ExtensionContext.storagePath`. The parent folder of `destination` may not exist, so make sure to created it
before writing the backup to this location.

#### Defined in

[index.d.ts:3930](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3930)
