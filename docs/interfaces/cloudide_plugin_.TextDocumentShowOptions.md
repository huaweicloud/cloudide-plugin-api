[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TextDocumentShowOptions

# Interface: TextDocumentShowOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TextDocumentShowOptions

Represents options to configure the behavior of showing a [document](#TextDocument) in an [editor](#TextEditor).

## Table of contents

### Properties

- [preserveFocus](cloudide_plugin_.TextDocumentShowOptions.md#preservefocus)
- [preview](cloudide_plugin_.TextDocumentShowOptions.md#preview)
- [selection](cloudide_plugin_.TextDocumentShowOptions.md#selection)
- [viewColumn](cloudide_plugin_.TextDocumentShowOptions.md#viewcolumn)

## Properties

### preserveFocus

• `Optional` **preserveFocus**: `boolean`

An optional flag that when `true` will stop the [editor](#TextEditor) from taking focus.

#### Defined in

[index.d.ts:10167](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10167)

___

### preview

• `Optional` **preview**: `boolean`

An optional flag that controls if an [editor](#TextEditor)-tab will be replaced
with the next editor or if it will be kept.

#### Defined in

[index.d.ts:10173](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10173)

___

### selection

• `Optional` **selection**: [`Range`](../classes/cloudide_plugin_.Range.md)

An optional selection to apply for the document in the [editor](#TextEditor).

#### Defined in

[index.d.ts:10178](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10178)

___

### viewColumn

• `Optional` **viewColumn**: [`ViewColumn`](../enums/cloudide_plugin_.ViewColumn.md)

An optional view column in which the [editor](#TextEditor) should be shown.
The default is the [active](#ViewColumn.Active), other values are adjusted to
be `Min(column, columnCount + 1)`, the [active](#ViewColumn.Active)-column is
not adjusted. Use [`ViewColumn.Beside`](#ViewColumn.Beside) to open the
editor to the side of the currently active one.

#### Defined in

[index.d.ts:10162](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10162)
