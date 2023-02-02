[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlineCompletionItem

# Class: InlineCompletionItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlineCompletionItem

An inline completion item represents a text snippet that is proposed inline to complete text that is being typed.

**`See`**

[provideInlineCompletionItems](../interfaces/codearts_plugin_.InlineCompletionItemProvider.md#provideinlinecompletionitems)

## Table of contents

### Constructors

- [constructor](codearts_plugin_.InlineCompletionItem.md#constructor)

### Properties

- [command](codearts_plugin_.InlineCompletionItem.md#command)
- [filterText](codearts_plugin_.InlineCompletionItem.md#filtertext)
- [insertText](codearts_plugin_.InlineCompletionItem.md#inserttext)
- [range](codearts_plugin_.InlineCompletionItem.md#range)

## Constructors

### constructor

• **new InlineCompletionItem**(`insertText`, `range?`, `command?`)

Creates a new inline completion item.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `insertText` | `string` \| [`SnippetString`](codearts_plugin_.SnippetString.md) | The text to replace the range with. |
| `range?` | [`Range`](codearts_plugin_.Range.md) | The range to replace. If not set, the word at the requested position will be used. |
| `command?` | [`Command`](../interfaces/codearts_plugin_.Command.md) | An optional [Command](../interfaces/codearts_plugin_.Command.md) that is executed *after* inserting this completion. |

#### Defined in

[index.d.ts:4665](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L4665)

## Properties

### command

• `Optional` **command**: [`Command`](../interfaces/codearts_plugin_.Command.md)

An optional [Command](../interfaces/codearts_plugin_.Command.md) that is executed *after* inserting this completion.

#### Defined in

[index.d.ts:4656](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L4656)

___

### filterText

• `Optional` **filterText**: `string`

A text that is used to decide if this inline completion should be shown. When `falsy`
the [insertText](codearts_plugin_.InlineCompletionItem.md#inserttext) is used.

An inline completion is shown if the text to replace is a prefix of the filter text.

#### Defined in

[index.d.ts:4643](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L4643)

___

### insertText

• **insertText**: `string` \| [`SnippetString`](codearts_plugin_.SnippetString.md)

The text to replace the range with. Must be set.
Is used both for the preview and the accept operation.

#### Defined in

[index.d.ts:4635](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L4635)

___

### range

• `Optional` **range**: [`Range`](codearts_plugin_.Range.md)

The range to replace.
Must begin and end on the same line.

Prefer replacements over insertions to provide a better experience when the user deletes typed text.

#### Defined in

[index.d.ts:4651](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L4651)
