[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CustomDocumentOpenContext

# Interface: CustomDocumentOpenContext

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CustomDocumentOpenContext

Additional information about the opening custom document.

## Table of contents

### Properties

- [backupId](cloudide_plugin_.CustomDocumentOpenContext.md#backupid)

## Properties

### backupId

• `Optional` `Readonly` **backupId**: `string`

The id of the backup to restore the document from or `undefined` if there is no backup.

If this is provided, your extension should restore the editor from the backup instead of reading the file
from the user's workspace.

#### Defined in

[index.d.ts:3844](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3844)
