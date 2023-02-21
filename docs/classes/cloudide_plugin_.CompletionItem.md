[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CompletionItem

# Class: CompletionItem

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CompletionItem

A completion item represents a text snippet that is proposed to complete text that is being typed.

It is sufficient to create a completion item from just a [label](#CompletionItem.label). In that
case the completion item will replace the [word](#TextDocument.getWordRangeAtPosition)
until the cursor with the given label or [insertText](#CompletionItem.insertText). Otherwise the
the given [edit](#CompletionItem.textEdit) is used.

When selecting a completion item in the editor its defined or synthesized text edit will be applied
to *all* cursors/selections whereas [additionalTextEdits](#additionalTextEdits) will be
applied as provided.

**`See`**

 - [CompletionItemProvider.provideCompletionItems](#CompletionItemProvider.provideCompletionItems)
 - [CompletionItemProvider.resolveCompletionItem](#CompletionItemProvider.resolveCompletionItem)

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.CompletionItem.md#constructor)

### Properties

- [additionalTextEdits](cloudide_plugin_.CompletionItem.md#additionaltextedits)
- [command](cloudide_plugin_.CompletionItem.md#command)
- [commitCharacters](cloudide_plugin_.CompletionItem.md#commitcharacters)
- [deprecated](cloudide_plugin_.CompletionItem.md#deprecated)
- [detail](cloudide_plugin_.CompletionItem.md#detail)
- [documentation](cloudide_plugin_.CompletionItem.md#documentation)
- [filterText](cloudide_plugin_.CompletionItem.md#filtertext)
- [insertText](cloudide_plugin_.CompletionItem.md#inserttext)
- [keepWhitespace](cloudide_plugin_.CompletionItem.md#keepwhitespace)
- [kind](cloudide_plugin_.CompletionItem.md#kind)
- [label](cloudide_plugin_.CompletionItem.md#label)
- [preselect](cloudide_plugin_.CompletionItem.md#preselect)
- [range](cloudide_plugin_.CompletionItem.md#range)
- [sortText](cloudide_plugin_.CompletionItem.md#sorttext)
- [tags](cloudide_plugin_.CompletionItem.md#tags)
- [textEdit](cloudide_plugin_.CompletionItem.md#textedit)

## Constructors

### constructor

• **new CompletionItem**(`label`, `kind?`)

Creates a new completion item.

Completion items must have at least a [label](#CompletionItem.label) which then
will be used as insert text as well as for sorting and filtering.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `label` | `string` | The label of the completion. |
| `kind?` | [`CompletionItemKind`](../enums/cloudide_plugin_.CompletionItemKind.md) | The [kind](#CompletionItemKind) of the completion. |

#### Defined in

[index.d.ts:7594](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7594)

## Properties

### additionalTextEdits

• `Optional` **additionalTextEdits**: [`TextEdit`](cloudide_plugin_.TextEdit.md)[]

An optional array of additional [text edits](#TextEdit) that are applied when
selecting this completion. Edits must not overlap with the main [edit](#CompletionItem.textEdit)
nor with themselves.

#### Defined in

[index.d.ts:7559](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7559)

___

### command

• `Optional` **command**: [`Command`](../interfaces/cloudide_plugin_.Command.md)

An optional [command](#Command) that is executed *after* inserting this completion. *Note* that
additional modifications to the current document should be described with the
[additionalTextEdits](#additionalTextEdits)-property.

#### Defined in

[index.d.ts:7566](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7566)

___

### commitCharacters

• `Optional` **commitCharacters**: `string`[]

An optional set of characters that when pressed while this completion is active will accept it first and
then type that character. *Note* that all commit characters should have `length=1` and that superfluous
characters will be ignored.

#### Defined in

[index.d.ts:7545](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7545)

___

### deprecated

• `Optional` **deprecated**: `boolean`

**`Deprecated`**

Use `CompletionItem.tags` instead.

#### Defined in

[index.d.ts:7583](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7583)

___

### detail

• `Optional` **detail**: `string`

A human-readable string with additional information
about this item, like type or symbol information.

#### Defined in

[index.d.ts:7487](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7487)

___

### documentation

• `Optional` **documentation**: `string` \| [`MarkdownString`](cloudide_plugin_.MarkdownString.md)

A human-readable string that represents a doc-comment.

#### Defined in

[index.d.ts:7497](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7497)

___

### filterText

• `Optional` **filterText**: `string`

A string that should be used when filtering a set of
completion items. When `falsy` the [label](#CompletionItem.label)
is used.

#### Defined in

[index.d.ts:7511](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7511)

___

### insertText

• `Optional` **insertText**: `string` \| [`SnippetString`](cloudide_plugin_.SnippetString.md)

A string or snippet that should be inserted in a document when selecting
this completion. When `falsy` the [label](#CompletionItem.label)
is used.

#### Defined in

[index.d.ts:7525](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7525)

___

### keepWhitespace

• `Optional` **keepWhitespace**: `boolean`

Keep whitespace of the [insertText](#CompletionItem.insertText) as is. By default, the editor adjusts leading
whitespace of new lines so that they match the indentation of the line for which the item is accepted - setting
this to `true` will prevent that.

#### Defined in

[index.d.ts:7552](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7552)

___

### kind

• `Optional` **kind**: [`CompletionItemKind`](../enums/cloudide_plugin_.CompletionItemKind.md)

The kind of this completion item. Based on the kind
an icon is chosen by the editor.

#### Defined in

[index.d.ts:7481](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7481)

___

### label

• **label**: `string`

The label of this completion item. By default
this is also the text that is inserted when selecting
this completion.

#### Defined in

[index.d.ts:7475](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7475)

___

### preselect

• `Optional` **preselect**: `boolean`

Select this item when showing. *Note* that only one completion item can be selected and
that the editor decides which item that is. The rule is that the *first* item of those
that match best is selected.

#### Defined in

[index.d.ts:7518](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7518)

___

### range

• `Optional` **range**: [`Range`](cloudide_plugin_.Range.md) \| { `inserting`: [`Range`](cloudide_plugin_.Range.md) ; `replacing`: [`Range`](cloudide_plugin_.Range.md)  }

A range or a insert and replace range selecting the text that should be replaced by this completion item.

When omitted, the range of the [current word](#TextDocument.getWordRangeAtPosition) is used as replace-range
and as insert-range the start of the [current word](#TextDocument.getWordRangeAtPosition) to the
current position is used.

*Note 1:* A range must be a [single line](#Range.isSingleLine) and it must
[contain](#Range.contains) the position at which completion has been [requested](#CompletionItemProvider.provideCompletionItems).
*Note 2:* A insert range must be a prefix of a replace range, that means it must be contained and starting at the same position.

#### Defined in

[index.d.ts:7538](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7538)

___

### sortText

• `Optional` **sortText**: `string`

A string that should be used when comparing this item
with other items. When `falsy` the [label](#CompletionItem.label)
is used.

#### Defined in

[index.d.ts:7504](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7504)

___

### tags

• `Optional` **tags**: readonly [`Deprecated`](../enums/cloudide_plugin_.CompletionItemTag.md#deprecated)[]

Tags for this completion item.

#### Defined in

[index.d.ts:7492](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7492)

___

### textEdit

• `Optional` **textEdit**: [`TextEdit`](cloudide_plugin_.TextEdit.md)

**`Deprecated`**

Use `CompletionItem.insertText` and `CompletionItem.range` instead.

~~An [edit](#TextEdit) which is applied to a document when selecting
this completion. When an edit is provided the value of
[insertText](#CompletionItem.insertText) is ignored.~~

~~The [range](#Range) of the edit must be single-line and on the same
line completions were [requested](#CompletionItemProvider.provideCompletionItems) at.~~

#### Defined in

[index.d.ts:7578](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7578)
