**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextEditor

# Interface: TextEditor

Represents an editor that is attached to a [document](#TextDocument).

## Hierarchy

* **TextEditor**

## Index

### Properties

* [document](_index_d_._plugin_.texteditor.md#document)
* [options](_index_d_._plugin_.texteditor.md#options)
* [selection](_index_d_._plugin_.texteditor.md#selection)
* [selections](_index_d_._plugin_.texteditor.md#selections)
* [viewColumn](_index_d_._plugin_.texteditor.md#viewcolumn)
* [visibleRanges](_index_d_._plugin_.texteditor.md#visibleranges)

### Methods

* [edit](_index_d_._plugin_.texteditor.md#edit)
* [hide](_index_d_._plugin_.texteditor.md#hide)
* [insertSnippet](_index_d_._plugin_.texteditor.md#insertsnippet)
* [revealRange](_index_d_._plugin_.texteditor.md#revealrange)
* [setDecorations](_index_d_._plugin_.texteditor.md#setdecorations)
* [show](_index_d_._plugin_.texteditor.md#show)

## Properties

### document

• `Readonly` **document**: [TextDocument](_index_d_._plugin_.textdocument.md)

*Defined in [index.d.ts:1216](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1216)*

The document associated with this text editor. The document will be the same for the entire lifetime of this text editor.

___

### options

•  **options**: [TextEditorOptions](_index_d_._plugin_.texteditoroptions.md)

*Defined in [index.d.ts:1237](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1237)*

Text editor options.

___

### selection

•  **selection**: [Selection](../classes/_index_d_._plugin_.selection.md)

*Defined in [index.d.ts:1221](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1221)*

The primary selection on this text editor. Shorthand for `TextEditor.selections[0]`.

___

### selections

•  **selections**: [Selection](../classes/_index_d_._plugin_.selection.md)[]

*Defined in [index.d.ts:1226](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1226)*

The selections in this text editor. The primary selection is always at index 0.

___

### viewColumn

• `Optional` `Readonly` **viewColumn**: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md)

*Defined in [index.d.ts:1244](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1244)*

The column in which this editor shows. Will be `undefined` in case this
isn't one of the main editors, e.g. an embedded editor, or when the editor
column is larger than three.

___

### visibleRanges

• `Readonly` **visibleRanges**: [Range](../classes/_index_d_._plugin_.range.md)[]

*Defined in [index.d.ts:1232](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1232)*

The current visible ranges in the editor (vertically).
This accounts only for vertical scrolling, and not for horizontal scrolling.

## Methods

### edit

▸ **edit**(`callback`: (editBuilder: [TextEditorEdit](_index_d_._plugin_.texteditoredit.md)) => void, `options?`: { undoStopAfter: boolean ; undoStopBefore: boolean  }): [Thenable](_index_d_.thenable.md)\<boolean>

*Defined in [index.d.ts:1257](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1257)*

Perform an edit on the document associated with this text editor.

The given callback-function is invoked with an [edit-builder](#TextEditorEdit) which must
be used to make edits. Note that the edit-builder is only valid while the
callback executes.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`callback` | (editBuilder: [TextEditorEdit](_index_d_._plugin_.texteditoredit.md)) => void | A function which can create edits using an [edit-builder](#TextEditorEdit). |
`options?` | { undoStopAfter: boolean ; undoStopBefore: boolean  } | The undo/redo behavior around this edit. By default, undo stops will be created before and after this edit. |

**Returns:** [Thenable](_index_d_.thenable.md)\<boolean>

A promise that resolves with a value indicating if the edits could be applied.

___

### hide

▸ **hide**(): void

*Defined in [index.d.ts:1307](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1307)*

Hide the text editor.

**`deprecated`** Use the command `workbench.action.closeActiveEditor` instead.
This method shows unexpected behavior and will be removed in the next major update.

**Returns:** void

___

### insertSnippet

▸ **insertSnippet**(`snippet`: [SnippetString](../classes/_index_d_._plugin_.snippetstring.md), `location?`: [Position](../classes/_index_d_._plugin_.position.md) \| [Range](../classes/_index_d_._plugin_.range.md) \| ReadonlyArray\<[Position](../classes/_index_d_._plugin_.position.md)> \| ReadonlyArray\<[Range](../classes/_index_d_._plugin_.range.md)>, `options?`: { undoStopAfter: boolean ; undoStopBefore: boolean  }): [Thenable](_index_d_.thenable.md)\<boolean>

*Defined in [index.d.ts:1270](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1270)*

Insert a [snippet](#SnippetString) and put the editor into snippet mode. "Snippet mode"
means the editor adds placeholders and additional cursors so that the user can complete
or accept the snippet.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`snippet` | [SnippetString](../classes/_index_d_._plugin_.snippetstring.md) | The snippet to insert in this edit. |
`location?` | [Position](../classes/_index_d_._plugin_.position.md) \| [Range](../classes/_index_d_._plugin_.range.md) \| ReadonlyArray\<[Position](../classes/_index_d_._plugin_.position.md)> \| ReadonlyArray\<[Range](../classes/_index_d_._plugin_.range.md)> | Position or range at which to insert the snippet, defaults to the current editor selection or selections. |
`options?` | { undoStopAfter: boolean ; undoStopBefore: boolean  } | The undo/redo behavior around this edit. By default, undo stops will be created before and after this edit. |

**Returns:** [Thenable](_index_d_.thenable.md)\<boolean>

A promise that resolves with a value indicating if the snippet could be inserted. Note that the promise does not signal
that the snippet is completely filled-in or accepted.

___

### revealRange

▸ **revealRange**(`range`: [Range](../classes/_index_d_._plugin_.range.md), `revealType?`: [TextEditorRevealType](../enums/_index_d_._plugin_.texteditorrevealtype.md)): void

*Defined in [index.d.ts:1289](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1289)*

Scroll as indicated by `revealType` in order to reveal the given range.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`range` | [Range](../classes/_index_d_._plugin_.range.md) | A range. |
`revealType?` | [TextEditorRevealType](../enums/_index_d_._plugin_.texteditorrevealtype.md) | The scrolling strategy for revealing `range`.  |

**Returns:** void

___

### setDecorations

▸ **setDecorations**(`decorationType`: [TextEditorDecorationType](_index_d_._plugin_.texteditordecorationtype.md), `rangesOrOptions`: [Range](../classes/_index_d_._plugin_.range.md)[] \| [DecorationOptions](_index_d_._plugin_.decorationoptions.md)[]): void

*Defined in [index.d.ts:1281](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1281)*

Adds a set of decorations to the text editor. If a set of decorations already exists with
the given [decoration type](#TextEditorDecorationType), they will be replaced.

**`see`** [createTextEditorDecorationType](#window.createTextEditorDecorationType).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`decorationType` | [TextEditorDecorationType](_index_d_._plugin_.texteditordecorationtype.md) | A decoration type. |
`rangesOrOptions` | [Range](../classes/_index_d_._plugin_.range.md)[] \| [DecorationOptions](_index_d_._plugin_.decorationoptions.md)[] | Either [ranges](#Range) or more detailed [options](#DecorationOptions).  |

**Returns:** void

___

### show

▸ **show**(`column?`: [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md)): void

*Defined in [index.d.ts:1299](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1299)*

Show the text editor.

**`deprecated`** Use [window.showTextDocument](#window.showTextDocument) instead.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`column?` | [ViewColumn](../enums/_index_d_._plugin_.viewcolumn.md) | The [column](#ViewColumn) in which to show this editor. This method shows unexpected behavior and will be removed in the next major update.  |

**Returns:** void
