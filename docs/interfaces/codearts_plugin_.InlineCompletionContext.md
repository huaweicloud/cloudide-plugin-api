[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlineCompletionContext

# Interface: InlineCompletionContext

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlineCompletionContext

Provides information about the context in which an inline completion was requested.

## Table of contents

### Properties

- [selectedCompletionInfo](codearts_plugin_.InlineCompletionContext.md#selectedcompletioninfo)
- [triggerKind](codearts_plugin_.InlineCompletionContext.md#triggerkind)

## Properties

### selectedCompletionInfo

• `Readonly` **selectedCompletionInfo**: `undefined` \| [`SelectedCompletionInfo`](codearts_plugin_.SelectedCompletionInfo.md)

Provides information about the currently selected item in the autocomplete widget if it is visible.

If set, provided inline completions must extend the text of the selected item
and use the same range, otherwise they are not shown as preview.
As an example, if the document text is `console.` and the selected item is `.log` replacing the `.` in the document,
the inline completion must also replace `.` and start with `.log`, for example `.log()`.

Inline completion providers are requested again whenever the selected item changes.

#### Defined in

[index.d.ts:4590](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L4590)

___

### triggerKind

• `Readonly` **triggerKind**: [`InlineCompletionTriggerKind`](../enums/codearts_plugin_.InlineCompletionTriggerKind.md)

Describes how the inline completion was triggered.

#### Defined in

[index.d.ts:4578](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L4578)
