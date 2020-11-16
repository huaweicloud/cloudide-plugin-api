**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CompletionItem

# Class: CompletionItem

A completion item represents a text snippet that is proposed to complete text that is being typed.

It is sufficient to create a completion item from just a [label](#CompletionItem.label). In that
case the completion item will replace the [word](#TextDocument.getWordRangeAtPosition)
until the cursor with the given label or [insertText](#CompletionItem.insertText). Otherwise the
given [edit](#CompletionItem.textEdit) is used.

When selecting a completion item in the editor its defined or synthesized text edit will be applied
to *all* cursors/selections whereas [additionalTextEdits](#CompletionItem.additionalTextEdits) will be
applied as provided.

**`see`** [CompletionItemProvider.provideCompletionItems](#CompletionItemProvider.provideCompletionItems)

**`see`** [CompletionItemProvider.resolveCompletionItem](#CompletionItemProvider.resolveCompletionItem)

## Hierarchy

* **CompletionItem**

## Index

### Constructors

* [constructor](_index_d_._plugin_.completionitem.md#constructor)

### Properties

* [additionalTextEdits](_index_d_._plugin_.completionitem.md#additionaltextedits)
* [command](_index_d_._plugin_.completionitem.md#command)
* [commitCharacters](_index_d_._plugin_.completionitem.md#commitcharacters)
* [detail](_index_d_._plugin_.completionitem.md#detail)
* [documentation](_index_d_._plugin_.completionitem.md#documentation)
* [filterText](_index_d_._plugin_.completionitem.md#filtertext)
* [insertText](_index_d_._plugin_.completionitem.md#inserttext)
* [keepWhitespace](_index_d_._plugin_.completionitem.md#keepwhitespace)
* [kind](_index_d_._plugin_.completionitem.md#kind)
* [label](_index_d_._plugin_.completionitem.md#label)
* [preselect](_index_d_._plugin_.completionitem.md#preselect)
* [range](_index_d_._plugin_.completionitem.md#range)
* [sortText](_index_d_._plugin_.completionitem.md#sorttext)
* [tags](_index_d_._plugin_.completionitem.md#tags)
* [textEdit](_index_d_._plugin_.completionitem.md#textedit)

## Constructors

### constructor

\+ **new CompletionItem**(`label`: string, `kind?`: [CompletionItemKind](../enums/_index_d_._plugin_.completionitemkind.md)): [CompletionItem](_index_d_._plugin_.completionitem.md)

*Defined in [index.d.ts:3851](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3851)*

Creates a new completion item.

Completion items must have at least a [label](#CompletionItem.label) which then
will be used as insert text as well as for sorting and filtering.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`label` | string | The label of the completion. |
`kind?` | [CompletionItemKind](../enums/_index_d_._plugin_.completionitemkind.md) | The [kind](#CompletionItemKind) of the completion.  |

**Returns:** [CompletionItem](_index_d_._plugin_.completionitem.md)

## Properties

### additionalTextEdits

• `Optional` **additionalTextEdits**: [TextEdit](_index_d_._plugin_.textedit.md)[]

*Defined in [index.d.ts:3844](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3844)*

An optional array of additional [text edits](#TextEdit) that are applied when
selecting this completion. Edits must not overlap with the main [edit](#CompletionItem.textEdit)
nor with themselves.

___

### command

• `Optional` **command**: [Command](../interfaces/_index_d_._plugin_.command.md)

*Defined in [index.d.ts:3851](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3851)*

An optional [command](#Command) that is executed *after* inserting this completion. *Note* that
additional modifications to the current document should be described with the
[additionalTextEdits](#CompletionItem.additionalTextEdits)-property.

___

### commitCharacters

• `Optional` **commitCharacters**: string[]

*Defined in [index.d.ts:3818](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3818)*

An optional set of characters that when pressed while this completion is active will accept it first and
then type that character. *Note* that all commit characters should have `length=1` and that superfluous
characters will be ignored.

___

### detail

• `Optional` **detail**: string

*Defined in [index.d.ts:3765](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3765)*

A human-readable string with additional information
about this item, like type or symbol information.

___

### documentation

• `Optional` **documentation**: string \| [MarkdownString](_index_d_._plugin_.markdownstring.md)

*Defined in [index.d.ts:3770](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3770)*

A human-readable string that represents a doc-comment.

___

### filterText

• `Optional` **filterText**: string

*Defined in [index.d.ts:3784](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3784)*

A string that should be used when filtering a set of
completion items. When `falsy` the [label](#CompletionItem.label)
is used.

___

### insertText

• `Optional` **insertText**: string \| [SnippetString](_index_d_._plugin_.snippetstring.md)

*Defined in [index.d.ts:3798](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3798)*

A string or snippet that should be inserted in a document when selecting
this completion. When `falsy` the [label](#CompletionItem.label)
is used.

___

### keepWhitespace

• `Optional` **keepWhitespace**: boolean

*Defined in [index.d.ts:3825](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3825)*

Keep whitespace of the [insertText](#CompletionItem.insertText) as is. By default, the editor adjusts leading
whitespace of new lines so that they match the indentation of the line for which the item is accepted - setting
this to `true` will prevent that.

___

### kind

• `Optional` **kind**: [CompletionItemKind](../enums/_index_d_._plugin_.completionitemkind.md)

*Defined in [index.d.ts:3754](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3754)*

The kind of this completion item. Based on the kind
an icon is chosen by the editor.

___

### label

•  **label**: string

*Defined in [index.d.ts:3748](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3748)*

The label of this completion item. By default
this is also the text that is inserted when selecting
this completion.

___

### preselect

• `Optional` **preselect**: boolean

*Defined in [index.d.ts:3791](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3791)*

Select this item when showing. *Note* that only one completion item can be selected and
that the editor decides which item that is. The rule is that the *first* item of those
that match best is selected.

___

### range

• `Optional` **range**: [Range](_index_d_._plugin_.range.md) \| { inserting: [Range](_index_d_._plugin_.range.md) ; replacing: [Range](_index_d_._plugin_.range.md)  }

*Defined in [index.d.ts:3811](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3811)*

A range or a insert and replace range selecting the text that should be replaced by this completion item.

When omitted, the range of the [current word](#TextDocument.getWordRangeAtPosition) is used as replace-range
and as insert-range the start of the [current word](#TextDocument.getWordRangeAtPosition) to the
current position is used.

*Note 1:* A range must be a [single line](#Range.isSingleLine) and it must
[contain](#Range.contains) the position at which completion has been [requested](#CompletionItemProvider.provideCompletionItems).
*Note 2:* A insert range must be a prefix of a replace range, that means it must be contained and starting at the same position.

___

### sortText

• `Optional` **sortText**: string

*Defined in [index.d.ts:3777](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3777)*

A string that should be used when comparing this item
with other items. When `falsy` the [label](#CompletionItem.label)
is used.

___

### tags

• `Optional` **tags**: ReadonlyArray\<[CompletionItemTag](../enums/_index_d_._plugin_.completionitemtag.md)>

*Defined in [index.d.ts:3759](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3759)*

Tags for this completion item.

___

### textEdit

• `Optional` **textEdit**: [TextEdit](_index_d_._plugin_.textedit.md)

*Defined in [index.d.ts:3837](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3837)*

**`deprecated`** Use `CompletionItem.insertText` and `CompletionItem.range` instead.

~~An [edit](#TextEdit) which is applied to a document when selecting
this completion. When an edit is provided the value of
[insertText](#CompletionItem.insertText) is ignored.~~

~~The [range](#Range) of the edit must be single-line and on the same
line completions were [requested](#CompletionItemProvider.provideCompletionItems) at.~~
