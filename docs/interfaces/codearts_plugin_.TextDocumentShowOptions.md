[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextDocumentShowOptions

# Interface: TextDocumentShowOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextDocumentShowOptions

Represents options to configure the behavior of showing a [document](codearts_plugin_.TextDocument.md) in an [editor](codearts_plugin_.TextEditor.md).

## Table of contents

### Properties

- [preserveFocus](codearts_plugin_.TextDocumentShowOptions.md#preservefocus)
- [preview](codearts_plugin_.TextDocumentShowOptions.md#preview)
- [selection](codearts_plugin_.TextDocumentShowOptions.md#selection)
- [viewColumn](codearts_plugin_.TextDocumentShowOptions.md#viewcolumn)

## Properties

### preserveFocus

• `Optional` **preserveFocus**: `boolean`

An optional flag that when `true` will stop the [editor](codearts_plugin_.TextEditor.md) from taking focus.

#### Defined in

[index.d.ts:773](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L773)

___

### preview

• `Optional` **preview**: `boolean`

An optional flag that controls if an [editor](codearts_plugin_.TextEditor.md)-tab shows as preview. Preview tabs will
be replaced and reused until set to stay - either explicitly or through editing.

*Note* that the flag is ignored if a user has disabled preview editors in settings.

#### Defined in

[index.d.ts:781](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L781)

___

### selection

• `Optional` **selection**: [`Range`](../classes/codearts_plugin_.Range.md)

An optional selection to apply for the document in the [editor](codearts_plugin_.TextEditor.md).

#### Defined in

[index.d.ts:786](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L786)

___

### viewColumn

• `Optional` **viewColumn**: [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md)

An optional view column in which the [editor](codearts_plugin_.TextEditor.md) should be shown.
The default is the [active](../enums/codearts_plugin_.ViewColumn.md#active), other values are adjusted to
be `Min(column, columnCount + 1)`, the [active](../enums/codearts_plugin_.ViewColumn.md#active)-column is
not adjusted. Use [`Beside`](../enums/codearts_plugin_.ViewColumn.md#beside) to open the
editor to the side of the currently active one.

#### Defined in

[index.d.ts:768](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L768)
