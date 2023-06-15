[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CustomDocumentOpenContext

# Interface: CustomDocumentOpenContext

["@codearts/plugin"](../modules/_codearts_plugin_.md).CustomDocumentOpenContext

Additional information about the opening custom document.

## Table of contents

### Properties

- [backupId](codearts_plugin_.CustomDocumentOpenContext.md#backupid)
- [untitledDocumentData](codearts_plugin_.CustomDocumentOpenContext.md#untitleddocumentdata)

## Properties

### backupId

• `Readonly` **backupId**: `undefined` \| `string`

The id of the backup to restore the document from or `undefined` if there is no backup.

If this is provided, your extension should restore the editor from the backup instead of reading the file
from the user's workspace.

#### Defined in

[index.d.ts:8902](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8902)

___

### untitledDocumentData

• `Readonly` **untitledDocumentData**: `undefined` \| `Uint8Array`

If the URI is an untitled file, this will be populated with the byte data of that file

If this is provided, your extension should utilize this byte data rather than executing fs APIs on the URI passed in

#### Defined in

[index.d.ts:8909](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L8909)
