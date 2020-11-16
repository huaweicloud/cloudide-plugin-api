**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextEditorEdit

# Interface: TextEditorEdit

A complex edit that will be applied in one transaction on a TextEditor.
This holds a description of the edits and if the edits are valid (i.e. no overlapping regions, document was not changed in the meantime, etc.)
they can be applied on a [document](#TextDocument) associated with a [text editor](#TextEditor).

## Hierarchy

* **TextEditorEdit**

## Index

### Methods

* [delete](_index_d_._plugin_.texteditoredit.md#delete)
* [insert](_index_d_._plugin_.texteditoredit.md#insert)
* [replace](_index_d_._plugin_.texteditoredit.md#replace)
* [setEndOfLine](_index_d_._plugin_.texteditoredit.md#setendofline)

## Methods

### delete

▸ **delete**(`location`: [Range](../classes/_index_d_._plugin_.range.md) \| [Selection](../classes/_index_d_._plugin_.selection.md)): void

*Defined in [index.d.ts:1233](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1233)*

Delete a certain text region.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`location` | [Range](../classes/_index_d_._plugin_.range.md) \| [Selection](../classes/_index_d_._plugin_.selection.md) | The range this operation should remove.  |

**Returns:** void

___

### insert

▸ **insert**(`location`: [Position](../classes/_index_d_._plugin_.position.md), `value`: string): void

*Defined in [index.d.ts:1226](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1226)*

Insert text at a location.
You can use \r\n or \n in `value` and they will be normalized to the current [document](#TextDocument).
Although the equivalent text edit can be made with [replace](#TextEditorEdit.replace), `insert` will produce a different resulting selection (it will get moved).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`location` | [Position](../classes/_index_d_._plugin_.position.md) | The position where the new text should be inserted. |
`value` | string | The new text this operation should insert.  |

**Returns:** void

___

### replace

▸ **replace**(`location`: [Position](../classes/_index_d_._plugin_.position.md) \| [Range](../classes/_index_d_._plugin_.range.md) \| [Selection](../classes/_index_d_._plugin_.selection.md), `value`: string): void

*Defined in [index.d.ts:1216](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1216)*

Replace a certain text region with a new value.
You can use \r\n or \n in `value` and they will be normalized to the current [document](#TextDocument).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`location` | [Position](../classes/_index_d_._plugin_.position.md) \| [Range](../classes/_index_d_._plugin_.range.md) \| [Selection](../classes/_index_d_._plugin_.selection.md) | The range this operation should remove. |
`value` | string | The new text this operation should insert after removing `location`.  |

**Returns:** void

___

### setEndOfLine

▸ **setEndOfLine**(`endOfLine`: [EndOfLine](../enums/_index_d_._plugin_.endofline.md)): void

*Defined in [index.d.ts:1240](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1240)*

Set the end of line sequence.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`endOfLine` | [EndOfLine](../enums/_index_d_._plugin_.endofline.md) | The new end of line for the [document](#TextDocument).  |

**Returns:** void
