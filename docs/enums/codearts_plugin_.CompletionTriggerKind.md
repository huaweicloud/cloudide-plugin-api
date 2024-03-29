[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CompletionTriggerKind

# Enumeration: CompletionTriggerKind

["@codearts/plugin"](../modules/_codearts_plugin_.md).CompletionTriggerKind

How a [completion provider](../interfaces/codearts_plugin_.CompletionItemProvider.md) was triggered

## Table of contents

### Enumeration Members

- [Invoke](codearts_plugin_.CompletionTriggerKind.md#invoke)
- [TriggerCharacter](codearts_plugin_.CompletionTriggerKind.md#triggercharacter)
- [TriggerForIncompleteCompletions](codearts_plugin_.CompletionTriggerKind.md#triggerforincompletecompletions)

## Enumeration Members

### Invoke

• **Invoke** = ``0``

Completion was triggered normally.

#### Defined in

[index.d.ts:4500](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4500)

___

### TriggerCharacter

• **TriggerCharacter** = ``1``

Completion was triggered by a trigger character.

#### Defined in

[index.d.ts:4504](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4504)

___

### TriggerForIncompleteCompletions

• **TriggerForIncompleteCompletions** = ``2``

Completion was re-triggered as current completion list is incomplete

#### Defined in

[index.d.ts:4508](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4508)
