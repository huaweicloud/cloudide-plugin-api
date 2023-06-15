[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextEditor

# Interface: TextEditor

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextEditor

Represents an editor that is attached to a [document](codearts_plugin_.TextDocument.md).

## Table of contents

### Properties

- [document](codearts_plugin_.TextEditor.md#document)
- [options](codearts_plugin_.TextEditor.md#options)
- [selection](codearts_plugin_.TextEditor.md#selection)
- [selections](codearts_plugin_.TextEditor.md#selections)
- [viewColumn](codearts_plugin_.TextEditor.md#viewcolumn)
- [visibleRanges](codearts_plugin_.TextEditor.md#visibleranges)

### Methods

- [edit](codearts_plugin_.TextEditor.md#edit)
- [hide](codearts_plugin_.TextEditor.md#hide)
- [insertSnippet](codearts_plugin_.TextEditor.md#insertsnippet)
- [revealRange](codearts_plugin_.TextEditor.md#revealrange)
- [setDecorations](codearts_plugin_.TextEditor.md#setdecorations)
- [show](codearts_plugin_.TextEditor.md#show)

## Properties

### document

• `Readonly` **document**: [`TextDocument`](codearts_plugin_.TextDocument.md)

The document associated with this text editor. The document will be the same for the entire lifetime of this text editor.

#### Defined in

[index.d.ts:1169](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1169)

___

### options

• **options**: [`TextEditorOptions`](codearts_plugin_.TextEditorOptions.md)

Text editor options.

#### Defined in

[index.d.ts:1190](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1190)

___

### selection

• **selection**: [`Selection`](../classes/codearts_plugin_.Selection.md)

The primary selection on this text editor. Shorthand for `TextEditor.selections[0]`.

#### Defined in

[index.d.ts:1174](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1174)

___

### selections

• **selections**: readonly [`Selection`](../classes/codearts_plugin_.Selection.md)[]

The selections in this text editor. The primary selection is always at index 0.

#### Defined in

[index.d.ts:1179](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1179)

___

### viewColumn

• `Readonly` **viewColumn**: `undefined` \| [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md)

The column in which this editor shows. Will be `undefined` in case this
isn't one of the main editors, e.g. an embedded editor, or when the editor
column is larger than three.

#### Defined in

[index.d.ts:1197](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1197)

___

### visibleRanges

• `Readonly` **visibleRanges**: readonly [`Range`](../classes/codearts_plugin_.Range.md)[]

The current visible ranges in the editor (vertically).
This accounts only for vertical scrolling, and not for horizontal scrolling.

#### Defined in

[index.d.ts:1185](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1185)

## Methods

### edit

▸ **edit**(`callback`, `options?`): [`Thenable`](Thenable.md)<`boolean`\>

Perform an edit on the document associated with this text editor.

The given callback-function is invoked with an [edit-builder](codearts_plugin_.TextEditorEdit.md) which must
be used to make edits. Note that the edit-builder is only valid while the
callback executes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`editBuilder`: [`TextEditorEdit`](codearts_plugin_.TextEditorEdit.md)) => `void` | A function which can create edits using an [edit-builder](codearts_plugin_.TextEditorEdit.md). |
| `options?` | `Object` | The undo/redo behavior around this edit. By default, undo stops will be created before and after this edit. |
| `options.undoStopAfter` | `boolean` | - |
| `options.undoStopBefore` | `boolean` | - |

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

A promise that resolves with a value indicating if the edits could be applied.

#### Defined in

[index.d.ts:1210](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1210)

___

### hide

▸ **hide**(): `void`

Hide the text editor.

**`Deprecated`**

Use the command `workbench.action.closeActiveEditor` instead.
This method shows unexpected behavior and will be removed in the next major update.

#### Returns

`void`

#### Defined in

[index.d.ts:1262](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1262)

___

### insertSnippet

▸ **insertSnippet**(`snippet`, `location?`, `options?`): [`Thenable`](Thenable.md)<`boolean`\>

Insert a [snippet](../classes/codearts_plugin_.SnippetString.md) and put the editor into snippet mode. "Snippet mode"
means the editor adds placeholders and additional cursors so that the user can complete
or accept the snippet.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `snippet` | [`SnippetString`](../classes/codearts_plugin_.SnippetString.md) | The snippet to insert in this edit. |
| `location?` | [`Range`](../classes/codearts_plugin_.Range.md) \| [`Position`](../classes/codearts_plugin_.Position.md) \| readonly [`Range`](../classes/codearts_plugin_.Range.md)[] \| readonly [`Position`](../classes/codearts_plugin_.Position.md)[] | Position or range at which to insert the snippet, defaults to the current editor selection or selections. |
| `options?` | `Object` | The undo/redo behavior around this edit. By default, undo stops will be created before and after this edit. |
| `options.undoStopAfter` | `boolean` | - |
| `options.undoStopBefore` | `boolean` | - |

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

A promise that resolves with a value indicating if the snippet could be inserted. Note that the promise does not signal
that the snippet is completely filled-in or accepted.

#### Defined in

[index.d.ts:1223](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1223)

___

### revealRange

▸ **revealRange**(`range`, `revealType?`): `void`

Scroll as indicated by `revealType` in order to reveal the given range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](../classes/codearts_plugin_.Range.md) | A range. |
| `revealType?` | [`TextEditorRevealType`](../enums/codearts_plugin_.TextEditorRevealType.md) | The scrolling strategy for revealing `range`. |

#### Returns

`void`

#### Defined in

[index.d.ts:1244](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1244)

___

### setDecorations

▸ **setDecorations**(`decorationType`, `rangesOrOptions`): `void`

Adds a set of decorations to the text editor. If a set of decorations already exists with
the given [decoration type](codearts_plugin_.TextEditorDecorationType.md), they will be replaced. If
`rangesOrOptions` is empty, the existing decorations with the given [decoration type](codearts_plugin_.TextEditorDecorationType.md)
will be removed.

**`See`**

[createTextEditorDecorationType](../modules/codearts_plugin_.window.md#createtexteditordecorationtype).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `decorationType` | [`TextEditorDecorationType`](codearts_plugin_.TextEditorDecorationType.md) | A decoration type. |
| `rangesOrOptions` | readonly [`Range`](../classes/codearts_plugin_.Range.md)[] \| readonly [`DecorationOptions`](codearts_plugin_.DecorationOptions.md)[] | Either [ranges](../classes/codearts_plugin_.Range.md) or more detailed [options](codearts_plugin_.DecorationOptions.md). |

#### Returns

`void`

#### Defined in

[index.d.ts:1236](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1236)

___

### show

▸ **show**(`column?`): `void`

Show the text editor.

**`Deprecated`**

Use [showTextDocument](../modules/codearts_plugin_.window.md#showtextdocument) instead.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `column?` | [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md) | The [column](../enums/codearts_plugin_.ViewColumn.md) in which to show this editor. This method shows unexpected behavior and will be removed in the next major update. |

#### Returns

`void`

#### Defined in

[index.d.ts:1254](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1254)
