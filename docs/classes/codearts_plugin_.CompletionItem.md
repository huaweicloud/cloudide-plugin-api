[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CompletionItem

# Class: CompletionItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).CompletionItem

A completion item represents a text snippet that is proposed to complete text that is being typed.

It is sufficient to create a completion item from just a [label](codearts_plugin_.CompletionItem.md#label). In that
case the completion item will replace the [word](../interfaces/codearts_plugin_.TextDocument.md#getwordrangeatposition)
until the cursor with the given label or [insertText](codearts_plugin_.CompletionItem.md#inserttext). Otherwise the
given [edit](codearts_plugin_.CompletionItem.md#textedit) is used.

When selecting a completion item in the editor its defined or synthesized text edit will be applied
to *all* cursors/selections whereas [additionalTextEdits](codearts_plugin_.CompletionItem.md#additionaltextedits) will be
applied as provided.

**`See`**

 - [provideCompletionItems](../interfaces/codearts_plugin_.CompletionItemProvider.md#providecompletionitems)
 - [resolveCompletionItem](../interfaces/codearts_plugin_.CompletionItemProvider.md#resolvecompletionitem)

## Table of contents

### Constructors

- [constructor](codearts_plugin_.CompletionItem.md#constructor)

### Properties

- [additionalReplaceEdits](codearts_plugin_.CompletionItem.md#additionalreplaceedits)
- [additionalTextEdits](codearts_plugin_.CompletionItem.md#additionaltextedits)
- [command](codearts_plugin_.CompletionItem.md#command)
- [commitCharacters](codearts_plugin_.CompletionItem.md#commitcharacters)
- [detail](codearts_plugin_.CompletionItem.md#detail)
- [documentation](codearts_plugin_.CompletionItem.md#documentation)
- [filterText](codearts_plugin_.CompletionItem.md#filtertext)
- [insertText](codearts_plugin_.CompletionItem.md#inserttext)
- [keepWhitespace](codearts_plugin_.CompletionItem.md#keepwhitespace)
- [kind](codearts_plugin_.CompletionItem.md#kind)
- [label](codearts_plugin_.CompletionItem.md#label)
- [preselect](codearts_plugin_.CompletionItem.md#preselect)
- [range](codearts_plugin_.CompletionItem.md#range)
- [replaceText](codearts_plugin_.CompletionItem.md#replacetext)
- [sortText](codearts_plugin_.CompletionItem.md#sorttext)
- [tags](codearts_plugin_.CompletionItem.md#tags)
- [textEdit](codearts_plugin_.CompletionItem.md#textedit)

## Constructors

### constructor

• **new CompletionItem**(`label`, `kind?`)

Creates a new completion item.

Completion items must have at least a [label](codearts_plugin_.CompletionItem.md#label) which then
will be used as insert text as well as for sorting and filtering.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `label` | `string` \| [`CompletionItemLabel`](../interfaces/codearts_plugin_.CompletionItemLabel.md) | The label of the completion. |
| `kind?` | [`CompletionItemKind`](../enums/codearts_plugin_.CompletionItemKind.md) | The [kind](../enums/codearts_plugin_.CompletionItemKind.md) of the completion. |

#### Defined in

[index.d.ts:4444](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4444)

## Properties

### additionalReplaceEdits

• `Optional` **additionalReplaceEdits**: [`TextEdit`](codearts_plugin_.TextEdit.md)[]

An optional array of additional text edits that are applied when
selecting this completion in replace mode. Edits must not overlap with the main edit
nor with themselves. Fallbacks to [additionalTextEdits](codearts_plugin_.CompletionItem.md#additionaltextedits) if `falsy`.

#### Defined in

[index.d.ts:4433](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4433)

___

### additionalTextEdits

• `Optional` **additionalTextEdits**: [`TextEdit`](codearts_plugin_.TextEdit.md)[]

An optional array of additional [text edits](codearts_plugin_.TextEdit.md) that are applied when
selecting this completion. Edits must not overlap with the main [edit](codearts_plugin_.CompletionItem.md#textedit)
nor with themselves.

#### Defined in

[index.d.ts:4413](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4413)

___

### command

• `Optional` **command**: [`Command`](../interfaces/codearts_plugin_.Command.md)

An optional [Command](../interfaces/codearts_plugin_.Command.md) that is executed *after* inserting this completion. *Note* that
additional modifications to the current document should be described with the
[additionalTextEdits](codearts_plugin_.CompletionItem.md#additionaltextedits)-property.

#### Defined in

[index.d.ts:4420](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4420)

___

### commitCharacters

• `Optional` **commitCharacters**: `string`[]

An optional set of characters that when pressed while this completion is active will accept it first and
then type that character. *Note* that all commit characters should have `length=1` and that superfluous
characters will be ignored.

#### Defined in

[index.d.ts:4387](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4387)

___

### detail

• `Optional` **detail**: `string`

A human-readable string with additional information
about this item, like type or symbol information.

#### Defined in

[index.d.ts:4324](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4324)

___

### documentation

• `Optional` **documentation**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

A human-readable string that represents a doc-comment.

#### Defined in

[index.d.ts:4329](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4329)

___

### filterText

• `Optional` **filterText**: `string`

A string that should be used when filtering a set of
completion items. When `falsy` the [label](codearts_plugin_.CompletionItem.md#label)
is used.

Note that the filter text is matched against the leading word (prefix) which is defined
by the [`range`](codearts_plugin_.CompletionItem.md#range)-property.

#### Defined in

[index.d.ts:4353](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4353)

___

### insertText

• `Optional` **insertText**: `string` \| [`SnippetString`](codearts_plugin_.SnippetString.md)

A string or snippet that should be inserted in a document when selecting
this completion. When `falsy` the [label](codearts_plugin_.CompletionItem.md#label)
is used.

#### Defined in

[index.d.ts:4367](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4367)

___

### keepWhitespace

• `Optional` **keepWhitespace**: `boolean`

Keep whitespace of the [insertText](codearts_plugin_.CompletionItem.md#inserttext) as is. By default, the editor adjusts leading
whitespace of new lines so that they match the indentation of the line for which the item is accepted - setting
this to `true` will prevent that.

#### Defined in

[index.d.ts:4394](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4394)

___

### kind

• `Optional` **kind**: [`CompletionItemKind`](../enums/codearts_plugin_.CompletionItemKind.md)

The kind of this completion item. Based on the kind
an icon is chosen by the editor.

#### Defined in

[index.d.ts:4313](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4313)

___

### label

• **label**: `string` \| [`CompletionItemLabel`](../interfaces/codearts_plugin_.CompletionItemLabel.md)

The label of this completion item. By default
this is also the text that is inserted when selecting
this completion.

#### Defined in

[index.d.ts:4307](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4307)

___

### preselect

• `Optional` **preselect**: `boolean`

Select this item when showing. *Note* that only one completion item can be selected and
that the editor decides which item that is. The rule is that the *first* item of those
that match best is selected.

#### Defined in

[index.d.ts:4360](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4360)

___

### range

• `Optional` **range**: [`Range`](codearts_plugin_.Range.md) \| { `inserting`: [`Range`](codearts_plugin_.Range.md) ; `replacing`: [`Range`](codearts_plugin_.Range.md)  }

A range or a insert and replace range selecting the text that should be replaced by this completion item.

When omitted, the range of the [current word](../interfaces/codearts_plugin_.TextDocument.md#getwordrangeatposition) is used as replace-range
and as insert-range the start of the [current word](../interfaces/codearts_plugin_.TextDocument.md#getwordrangeatposition) to the
current position is used.

*Note 1:* A range must be a [single line](codearts_plugin_.Range.md#issingleline) and it must
[contain](codearts_plugin_.Range.md#contains) the position at which completion has been [requested](../interfaces/codearts_plugin_.CompletionItemProvider.md#providecompletionitems).
*Note 2:* A insert range must be a prefix of a replace range, that means it must be contained and starting at the same position.

#### Defined in

[index.d.ts:4380](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4380)

___

### replaceText

• `Optional` **replaceText**: `string` \| [`SnippetString`](codearts_plugin_.SnippetString.md)

A string or snippet that should be inserted in a document when selecting
this completion in replace mode. Fallbacks to [insertText](codearts_plugin_.CompletionItem.md#inserttext) if `falsy`.

#### Defined in

[index.d.ts:4426](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4426)

___

### sortText

• `Optional` **sortText**: `string`

A string that should be used when comparing this item
with other items. When `falsy` the [label](codearts_plugin_.CompletionItem.md#label)
is used.

Note that `sortText` is only used for the initial ordering of completion
items. When having a leading word (prefix) ordering is based on how
well completions match that prefix and the initial ordering is only used
when completions match equally well. The prefix is defined by the
[`range`](codearts_plugin_.CompletionItem.md#range)-property and can therefore be different
for each completion.

#### Defined in

[index.d.ts:4343](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4343)

___

### tags

• `Optional` **tags**: readonly [`Deprecated`](../enums/codearts_plugin_.CompletionItemTag.md#deprecated)[]

Tags for this completion item.

#### Defined in

[index.d.ts:4318](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4318)

___

### textEdit

• `Optional` **textEdit**: [`TextEdit`](codearts_plugin_.TextEdit.md)

**`Deprecated`**

Use `CompletionItem.insertText` and `CompletionItem.range` instead.

An [edit](codearts_plugin_.TextEdit.md) which is applied to a document when selecting
this completion. When an edit is provided the value of
[insertText](codearts_plugin_.CompletionItem.md#inserttext) is ignored.

The [Range](codearts_plugin_.Range.md) of the edit must be single-line and on the same
line completions were [requested](../interfaces/codearts_plugin_.CompletionItemProvider.md#providecompletionitems) at.

#### Defined in

[index.d.ts:4406](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4406)
