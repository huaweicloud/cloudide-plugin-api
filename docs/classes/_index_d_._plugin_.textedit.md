**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextEdit

# Class: TextEdit

A text edit represents edits that should be applied
to a document.

## Hierarchy

* **TextEdit**

## Index

### Constructors

* [constructor](_index_d_._plugin_.textedit.md#constructor)

### Properties

* [newEol](_index_d_._plugin_.textedit.md#neweol)
* [newText](_index_d_._plugin_.textedit.md#newtext)
* [range](_index_d_._plugin_.textedit.md#range)

### Methods

* [delete](_index_d_._plugin_.textedit.md#delete)
* [insert](_index_d_._plugin_.textedit.md#insert)
* [replace](_index_d_._plugin_.textedit.md#replace)
* [setEndOfLine](_index_d_._plugin_.textedit.md#setendofline)

## Constructors

### constructor

\+ **new TextEdit**(`range`: [Range](_index_d_._plugin_.range.md), `newText`: string): [TextEdit](_index_d_._plugin_.textedit.md)

*Defined in [index.d.ts:3158](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3158)*

Create a new TextEdit.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`range` | [Range](_index_d_._plugin_.range.md) | A range. |
`newText` | string | A string.  |

**Returns:** [TextEdit](_index_d_._plugin_.textedit.md)

## Properties

### newEol

• `Optional` **newEol**: [EndOfLine](../enums/_index_d_._plugin_.endofline.md)

*Defined in [index.d.ts:3158](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3158)*

The eol-sequence used in the document.

*Note* that the eol-sequence will be applied to the
whole document.

___

### newText

•  **newText**: string

*Defined in [index.d.ts:3150](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3150)*

The string this edit will insert.

___

### range

•  **range**: [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:3145](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3145)*

The range this edit applies to.

## Methods

### delete

▸ `Static`**delete**(`range`: [Range](_index_d_._plugin_.range.md)): [TextEdit](_index_d_._plugin_.textedit.md)

*Defined in [index.d.ts:3132](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3132)*

Utility to create a delete edit.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`range` | [Range](_index_d_._plugin_.range.md) | A range. |

**Returns:** [TextEdit](_index_d_._plugin_.textedit.md)

A new text edit object.

___

### insert

▸ `Static`**insert**(`position`: [Position](_index_d_._plugin_.position.md), `newText`: string): [TextEdit](_index_d_._plugin_.textedit.md)

*Defined in [index.d.ts:3124](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3124)*

Utility to create an insert edit.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`position` | [Position](_index_d_._plugin_.position.md) | A position, will become an empty range. |
`newText` | string | A string. |

**Returns:** [TextEdit](_index_d_._plugin_.textedit.md)

A new text edit object.

___

### replace

▸ `Static`**replace**(`range`: [Range](_index_d_._plugin_.range.md), `newText`: string): [TextEdit](_index_d_._plugin_.textedit.md)

*Defined in [index.d.ts:3115](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3115)*

Utility to create a replace edit.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`range` | [Range](_index_d_._plugin_.range.md) | A range. |
`newText` | string | A string. |

**Returns:** [TextEdit](_index_d_._plugin_.textedit.md)

A new text edit object.

___

### setEndOfLine

▸ `Static`**setEndOfLine**(`eol`: [EndOfLine](../enums/_index_d_._plugin_.endofline.md)): [TextEdit](_index_d_._plugin_.textedit.md)

*Defined in [index.d.ts:3140](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3140)*

Utility to create an eol-edit.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`eol` | [EndOfLine](../enums/_index_d_._plugin_.endofline.md) | An eol-sequence |

**Returns:** [TextEdit](_index_d_._plugin_.textedit.md)

A new text edit object.
