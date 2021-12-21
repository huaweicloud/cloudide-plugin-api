**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextDocumentShowOptions

# Interface: TextDocumentShowOptions

Represents options to configure the behavior of showing a [document](#TextDocument) in an [editor](#TextEditor).

## Hierarchy

* **TextDocumentShowOptions**

## Index

### Properties

* [preserveFocus](_index_d_._plugin_.textdocumentshowoptions.md#preservefocus)
* [preview](_index_d_._plugin_.textdocumentshowoptions.md#preview)
* [selection](_index_d_._plugin_.textdocumentshowoptions.md#selection)
* [viewColumn](_index_d_._plugin_.textdocumentshowoptions.md#viewcolumn)

## Properties

### preserveFocus

• `Optional` **preserveFocus**: boolean

*Defined in [index.d.ts:883](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L883)*

An optional flag that when `true` will stop the [editor](#TextEditor) from taking focus.

___

### preview

• `Optional` **preview**: boolean

*Defined in [index.d.ts:889](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L889)*

An optional flag that controls if an [editor](#TextEditor)-tab will be replaced
with the next editor or if it will be kept.

___

### selection

• `Optional` **selection**: [Range](../classes/_index_d_._plugin_.range.md)

*Defined in [index.d.ts:894](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L894)*

An optional selection to apply for the document in the [editor](#TextEditor).

___

### viewColumn

• `Optional` **viewColumn**: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md)

*Defined in [index.d.ts:878](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L878)*

An optional view column in which the [editor](#TextEditor) should be shown.
The default is the [active](#ViewColumn.Active), other values are adjusted to
be `Min(column, columnCount + 1)`, the [active](#ViewColumn.Active)-column is
not adjusted. Use [`ViewColumn.Beside`](#ViewColumn.Beside) to open the
editor to the side of the currently active one.
