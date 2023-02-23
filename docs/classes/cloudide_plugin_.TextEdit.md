[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TextEdit

# Class: TextEdit

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TextEdit

A text edit represents edits that should be applied
to a document.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.TextEdit.md#constructor)

### Properties

- [newEol](cloudide_plugin_.TextEdit.md#neweol)
- [newText](cloudide_plugin_.TextEdit.md#newtext)
- [range](cloudide_plugin_.TextEdit.md#range)

### Methods

- [delete](cloudide_plugin_.TextEdit.md#delete)
- [insert](cloudide_plugin_.TextEdit.md#insert)
- [replace](cloudide_plugin_.TextEdit.md#replace)
- [setEndOfLine](cloudide_plugin_.TextEdit.md#setendofline)

## Constructors

### constructor

• **new TextEdit**(`range`, `newText`)

Create a new TextEdit.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](cloudide_plugin_.Range.md) | A range. |
| `newText` | `string` | A string. |

#### Defined in

[index.d.ts:7405](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7405)

## Properties

### newEol

• **newEol**: [`EndOfLine`](../enums/cloudide_plugin_.EndOfLine.md)

The eol-sequence used in the document.

*Note* that the eol-sequence will be applied to the
whole document.

#### Defined in

[index.d.ts:7397](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7397)

___

### newText

• **newText**: `string`

The string this edit will insert.

#### Defined in

[index.d.ts:7389](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7389)

___

### range

• **range**: [`Range`](cloudide_plugin_.Range.md)

The range this edit applies to.

#### Defined in

[index.d.ts:7384](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7384)

## Methods

### delete

▸ `Static` **delete**(`range`): [`TextEdit`](cloudide_plugin_.TextEdit.md)

Utility to create a delete edit.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](cloudide_plugin_.Range.md) | A range. |

#### Returns

[`TextEdit`](cloudide_plugin_.TextEdit.md)

A new text edit object.

#### Defined in

[index.d.ts:7371](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7371)

___

### insert

▸ `Static` **insert**(`position`, `newText`): [`TextEdit`](cloudide_plugin_.TextEdit.md)

Utility to create an insert edit.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Position`](cloudide_plugin_.Position.md) | A position, will become an empty range. |
| `newText` | `string` | A string. |

#### Returns

[`TextEdit`](cloudide_plugin_.TextEdit.md)

A new text edit object.

#### Defined in

[index.d.ts:7363](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7363)

___

### replace

▸ `Static` **replace**(`range`, `newText`): [`TextEdit`](cloudide_plugin_.TextEdit.md)

Utility to create a replace edit.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](cloudide_plugin_.Range.md) | A range. |
| `newText` | `string` | A string. |

#### Returns

[`TextEdit`](cloudide_plugin_.TextEdit.md)

A new text edit object.

#### Defined in

[index.d.ts:7354](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7354)

___

### setEndOfLine

▸ `Static` **setEndOfLine**(`eol`): [`TextEdit`](cloudide_plugin_.TextEdit.md)

Utility to create an eol-edit.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `eol` | [`EndOfLine`](../enums/cloudide_plugin_.EndOfLine.md) | An eol-sequence |

#### Returns

[`TextEdit`](cloudide_plugin_.TextEdit.md)

A new text edit object.

#### Defined in

[index.d.ts:7379](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7379)
