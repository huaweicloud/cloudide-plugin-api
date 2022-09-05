[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CustomDocumentBackupContext

# Interface: CustomDocumentBackupContext

["@codearts/plugin"](../modules/_codearts_plugin_.md).CustomDocumentBackupContext

Additional information used to implement CustomEditableDocument.backup.

## Table of contents

### Properties

- [destination](codearts_plugin_.CustomDocumentBackupContext.md#destination)

## Properties

### destination

• `Readonly` **destination**: [`Uri`](../classes/codearts_plugin_.Uri.md)

Suggested file location to write the new backup.

Note that your extension is free to ignore this and use its own strategy for backup.

If the editor is for a resource from the current workspace, `destination` will point to a file inside
`ExtensionContext.storagePath`. The parent folder of `destination` may not exist, so make sure to created it
before writing the backup to this location.

#### Defined in

[index.d.ts:8791](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L8791)
