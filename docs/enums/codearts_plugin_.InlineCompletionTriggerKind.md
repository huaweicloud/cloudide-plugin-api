[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlineCompletionTriggerKind

# Enumeration: InlineCompletionTriggerKind

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlineCompletionTriggerKind

Describes how an [inline completion provider](../interfaces/codearts_plugin_.InlineCompletionItemProvider.md) was triggered.

## Table of contents

### Enumeration Members

- [Automatic](codearts_plugin_.InlineCompletionTriggerKind.md#automatic)
- [Invoke](codearts_plugin_.InlineCompletionTriggerKind.md#invoke)

## Enumeration Members

### Automatic

• **Automatic** = ``1``

Completion was triggered automatically while editing.
It is sufficient to return a single completion item in this case.

#### Defined in

[index.d.ts:4673](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4673)

___

### Invoke

• **Invoke** = ``0``

Completion was triggered explicitly by a user gesture.
Return multiple completion items to enable cycling through them.

#### Defined in

[index.d.ts:4667](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4667)
