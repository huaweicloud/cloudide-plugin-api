[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CompletionTriggerKind

# Enumeration: CompletionTriggerKind

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CompletionTriggerKind

How a [completion provider](#CompletionItemProvider) was triggered

## Table of contents

### Enumeration Members

- [Invoke](cloudide_plugin_.CompletionTriggerKind.md#invoke)
- [TriggerCharacter](cloudide_plugin_.CompletionTriggerKind.md#triggercharacter)
- [TriggerForIncompleteCompletions](cloudide_plugin_.CompletionTriggerKind.md#triggerforincompletecompletions)

## Enumeration Members

### Invoke

• **Invoke** = ``0``

Completion was triggered normally.

#### Defined in

[index.d.ts:6908](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6908)

___

### TriggerCharacter

• **TriggerCharacter** = ``1``

Completion was triggered by a trigger character.

#### Defined in

[index.d.ts:6912](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6912)

___

### TriggerForIncompleteCompletions

• **TriggerForIncompleteCompletions** = ``2``

Completion was re-triggered as current completion list is incomplete

#### Defined in

[index.d.ts:6916](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6916)
