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

[index.d.ts:4602](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L4602)

___

### Invoke

• **Invoke** = ``0``

Completion was triggered explicitly by a user gesture.
Return multiple completion items to enable cycling through them.

#### Defined in

[index.d.ts:4596](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L4596)
