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

[index.d.ts:4487](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L4487)

___

### TriggerCharacter

• **TriggerCharacter** = ``1``

Completion was triggered by a trigger character.

#### Defined in

[index.d.ts:4491](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L4491)

___

### TriggerForIncompleteCompletions

• **TriggerForIncompleteCompletions** = ``2``

Completion was re-triggered as current completion list is incomplete

#### Defined in

[index.d.ts:4495](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L4495)
