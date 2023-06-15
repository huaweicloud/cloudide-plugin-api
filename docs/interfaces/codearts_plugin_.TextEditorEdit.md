[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextEditorEdit

# Interface: TextEditorEdit

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextEditorEdit

A complex edit that will be applied in one transaction on a TextEditor.
This holds a description of the edits and if the edits are valid (i.e. no overlapping regions, document was not changed in the meantime, etc.)
they can be applied on a [document](codearts_plugin_.TextDocument.md) associated with a [text editor](codearts_plugin_.TextEditor.md).

## Table of contents

### Methods

- [delete](codearts_plugin_.TextEditorEdit.md#delete)
- [insert](codearts_plugin_.TextEditorEdit.md#insert)
- [replace](codearts_plugin_.TextEditorEdit.md#replace)
- [setEndOfLine](codearts_plugin_.TextEditorEdit.md#setendofline)

## Methods

### delete

▸ **delete**(`location`): `void`

Delete a certain text region.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `location` | [`Range`](../classes/codearts_plugin_.Range.md) \| [`Selection`](../classes/codearts_plugin_.Selection.md) | The range this operation should remove. |

#### Returns

`void`

#### Defined in

[index.d.ts:1309](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1309)

___

### insert

▸ **insert**(`location`, `value`): `void`

Insert text at a location.
You can use \r\n or \n in `value` and they will be normalized to the current [document](codearts_plugin_.TextDocument.md).
Although the equivalent text edit can be made with [replace](codearts_plugin_.TextEditorEdit.md#replace), `insert` will produce a different resulting selection (it will get moved).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `location` | [`Position`](../classes/codearts_plugin_.Position.md) | The position where the new text should be inserted. |
| `value` | `string` | The new text this operation should insert. |

#### Returns

`void`

#### Defined in

[index.d.ts:1302](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1302)

___

### replace

▸ **replace**(`location`, `value`): `void`

Replace a certain text region with a new value.
You can use \r\n or \n in `value` and they will be normalized to the current [document](codearts_plugin_.TextDocument.md).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `location` | [`Range`](../classes/codearts_plugin_.Range.md) \| [`Position`](../classes/codearts_plugin_.Position.md) \| [`Selection`](../classes/codearts_plugin_.Selection.md) | The range this operation should remove. |
| `value` | `string` | The new text this operation should insert after removing `location`. |

#### Returns

`void`

#### Defined in

[index.d.ts:1292](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1292)

___

### setEndOfLine

▸ **setEndOfLine**(`endOfLine`): `void`

Set the end of line sequence.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `endOfLine` | [`EndOfLine`](../enums/codearts_plugin_.EndOfLine.md) | The new end of line for the [document](codearts_plugin_.TextDocument.md). |

#### Returns

`void`

#### Defined in

[index.d.ts:1316](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1316)
