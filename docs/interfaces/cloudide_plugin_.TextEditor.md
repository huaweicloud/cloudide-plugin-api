[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TextEditor

# Interface: TextEditor

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TextEditor

Represents a text editor.
To close editor use 'workbench.action.closeActiveEditor' command.

## Table of contents

### Properties

- [document](cloudide_plugin_.TextEditor.md#document)
- [options](cloudide_plugin_.TextEditor.md#options)
- [selection](cloudide_plugin_.TextEditor.md#selection)
- [selections](cloudide_plugin_.TextEditor.md#selections)
- [viewColumn](cloudide_plugin_.TextEditor.md#viewcolumn)
- [visibleRanges](cloudide_plugin_.TextEditor.md#visibleranges)

### Methods

- [edit](cloudide_plugin_.TextEditor.md#edit)
- [insertSnippet](cloudide_plugin_.TextEditor.md#insertsnippet)
- [revealRange](cloudide_plugin_.TextEditor.md#revealrange)
- [setDecorations](cloudide_plugin_.TextEditor.md#setdecorations)

## Properties

### document

• `Readonly` **document**: [`TextDocument`](cloudide_plugin_.TextDocument.md)

The document associated with this text editor. The document will be the same for the entire lifetime of this text editor.

#### Defined in

[index.d.ts:1168](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1168)

___

### options

• **options**: [`TextEditorOptions`](cloudide_plugin_.TextEditorOptions.md)

Text editor options.

#### Defined in

[index.d.ts:1189](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1189)

___

### selection

• **selection**: [`Selection`](../classes/cloudide_plugin_.Selection.md)

The primary selection on this text editor. Shorthand for `TextEditor.selections[0]`.

#### Defined in

[index.d.ts:1173](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1173)

___

### selections

• **selections**: [`Selection`](../classes/cloudide_plugin_.Selection.md)[]

The selections in this text editor. The primary selection is always at index 0.

#### Defined in

[index.d.ts:1178](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1178)

___

### viewColumn

• `Optional` **viewColumn**: [`ViewColumn`](../enums/cloudide_plugin_.ViewColumn.md)

The column in which this editor shows. Will be `undefined` in case this
isn't one of the three main editors, e.g an embedded editor.

#### Defined in

[index.d.ts:1195](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1195)

___

### visibleRanges

• `Readonly` **visibleRanges**: [`Range`](../classes/cloudide_plugin_.Range.md)[]

The current visible ranges in the editor (vertically).
This accounts only for vertical scrolling, and not for horizontal scrolling.

#### Defined in

[index.d.ts:1184](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1184)

## Methods

### edit

▸ **edit**(`callback`, `options?`): `PromiseLike`<`boolean`\>

Perform an edit on the document associated with this text editor.

The given callback-function is invoked with an [edit-builder](#TextEditorEdit) which must
be used to make edits. Note that the edit-builder is only valid while the
callback executes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`editBuilder`: [`TextEditorEdit`](cloudide_plugin_.TextEditorEdit.md)) => `void` | A function which can create edits using an [edit-builder](#TextEditorEdit). |
| `options?` | `Object` | The undo/redo behavior around this edit. By default, undo stops will be created before and after this edit. |
| `options.undoStopAfter` | `boolean` | - |
| `options.undoStopBefore` | `boolean` | - |

#### Returns

`PromiseLike`<`boolean`\>

A promise that resolves with a value indicating if the edits could be applied.

#### Defined in

[index.d.ts:1208](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1208)

___

### insertSnippet

▸ **insertSnippet**(`snippet`, `location?`, `options?`): `PromiseLike`<`boolean`\>

Insert a [snippet](#SnippetString) and put the editor into snippet mode. "Snippet mode"
means the editor adds placeholders and additional cursors so that the user can complete
or accept the snippet.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `snippet` | [`SnippetString`](../classes/cloudide_plugin_.SnippetString.md) | The snippet to insert in this edit. |
| `location?` | [`Position`](../classes/cloudide_plugin_.Position.md) \| [`Range`](../classes/cloudide_plugin_.Range.md) \| [`Range`](../classes/cloudide_plugin_.Range.md)[] \| [`Position`](../classes/cloudide_plugin_.Position.md)[] | Position or range at which to insert the snippet, defaults to the current editor selection or selections. |
| `options?` | `Object` | The undo/redo behavior around this edit. By default, undo stops will be created before and after this edit. |
| `options.undoStopAfter` | `boolean` | - |
| `options.undoStopBefore` | `boolean` | - |

#### Returns

`PromiseLike`<`boolean`\>

A promise that resolves with a value indicating if the snippet could be inserted. Note that the promise does not signal
that the snippet is completely filled-in or accepted.

#### Defined in

[index.d.ts:1221](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1221)

___

### revealRange

▸ **revealRange**(`range`, `revealType?`): `void`

Scroll as indicated by `revealType` in order to reveal the given range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](../classes/cloudide_plugin_.Range.md) | A range. |
| `revealType?` | [`TextEditorRevealType`](../enums/cloudide_plugin_.TextEditorRevealType.md) | The scrolling strategy for revealing `range`. |

#### Returns

`void`

#### Defined in

[index.d.ts:1240](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1240)

___

### setDecorations

▸ **setDecorations**(`decorationType`, `rangesOrOptions`): `void`

Adds a set of decorations to the text editor. If a set of decorations already exists with
the given [decoration type](#TextEditorDecorationType), they will be replaced.

**`See`**

[createTextEditorDecorationType](#window.createTextEditorDecorationType).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `decorationType` | [`TextEditorDecorationType`](cloudide_plugin_.TextEditorDecorationType.md) | A decoration type. |
| `rangesOrOptions` | [`Range`](../classes/cloudide_plugin_.Range.md)[] \| [`DecorationOptions`](cloudide_plugin_.DecorationOptions.md)[] | Either [ranges](#Range) or more detailed [options](#DecorationOptions). |

#### Returns

`void`

#### Defined in

[index.d.ts:1232](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1232)
