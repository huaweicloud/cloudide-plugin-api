[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextEditorEdit

# Interface: TextEditorEdit

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextEditorEdit

## Table of contents

### Methods

- [delete](codearts_plugin_.TextEditorEdit.md#delete)
- [insert](codearts_plugin_.TextEditorEdit.md#insert)
- [replace](codearts_plugin_.TextEditorEdit.md#replace)
- [setEndOfLine](codearts_plugin_.TextEditorEdit.md#setendofline)

## Methods

### delete

▸ **delete**(`location`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `location` | [`Range`](../classes/codearts_plugin_.Range.md) \| [`Selection`](../classes/codearts_plugin_.Selection.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:1309](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L1309)

___

### insert

▸ **insert**(`location`, `value`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `location` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `value` | `string` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:1302](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L1302)

___

### replace

▸ **replace**(`location`, `value`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `location` | [`Range`](../classes/codearts_plugin_.Range.md) \| [`Position`](../classes/codearts_plugin_.Position.md) \| [`Selection`](../classes/codearts_plugin_.Selection.md) |  |
| `value` | `string` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:1292](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L1292)

___

### setEndOfLine

▸ **setEndOfLine**(`endOfLine`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `endOfLine` | [`EndOfLine`](../enums/codearts_plugin_.EndOfLine.md) |  |

#### Returns

`void`

#### Defined in

[index.d.ts:1316](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L1316)
