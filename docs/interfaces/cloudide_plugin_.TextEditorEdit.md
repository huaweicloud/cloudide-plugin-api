[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TextEditorEdit

# Interface: TextEditorEdit

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TextEditorEdit

## Table of contents

### Methods

- [delete](cloudide_plugin_.TextEditorEdit.md#delete)
- [insert](cloudide_plugin_.TextEditorEdit.md#insert)
- [replace](cloudide_plugin_.TextEditorEdit.md#replace)
- [setEndOfLine](cloudide_plugin_.TextEditorEdit.md#setendofline)

## Methods

### delete

▸ **delete**(`location`): `void`

Delete a certain text region.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `location` | [`Range`](../classes/cloudide_plugin_.Range.md) \| [`Selection`](../classes/cloudide_plugin_.Selection.md) | The range this operation should remove. |

#### Returns

`void`

#### Defined in

[index.d.ts:1271](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1271)

___

### insert

▸ **insert**(`location`, `value`): `void`

Insert text at a location.
You can use \r\n or \n in `value` and they will be normalized to the current [document](#TextDocument).
Although the equivalent text edit can be made with [replace](#TextEditorEdit.replace), `insert` will produce a different resulting selection (it will get moved).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `location` | [`Position`](../classes/cloudide_plugin_.Position.md) | The position where the new text should be inserted. |
| `value` | `string` | The new text this operation should insert. |

#### Returns

`void`

#### Defined in

[index.d.ts:1264](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1264)

___

### replace

▸ **replace**(`location`, `value`): `void`

Replace a certain text region with a new value.
You can use \r\n or \n in `value` and they will be normalized to the current [document](#TextDocument).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `location` | [`Position`](../classes/cloudide_plugin_.Position.md) \| [`Range`](../classes/cloudide_plugin_.Range.md) \| [`Selection`](../classes/cloudide_plugin_.Selection.md) | The range this operation should remove. |
| `value` | `string` | The new text this operation should insert after removing `location`. |

#### Returns

`void`

#### Defined in

[index.d.ts:1254](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1254)

___

### setEndOfLine

▸ **setEndOfLine**(`endOfLine`): `void`

Set the end of line sequence.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `endOfLine` | [`EndOfLine`](../enums/cloudide_plugin_.EndOfLine.md) | The new end of line for the [document](#TextDocument). |

#### Returns

`void`

#### Defined in

[index.d.ts:1278](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1278)
