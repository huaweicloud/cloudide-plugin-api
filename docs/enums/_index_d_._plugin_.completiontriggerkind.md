**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CompletionTriggerKind

# Enumeration: CompletionTriggerKind

How a [completion provider](#CompletionItemProvider) was triggered

## Index

### Enumeration members

* [Invoke](_index_d_._plugin_.completiontriggerkind.md#invoke)
* [TriggerCharacter](_index_d_._plugin_.completiontriggerkind.md#triggercharacter)
* [TriggerForIncompleteCompletions](_index_d_._plugin_.completiontriggerkind.md#triggerforincompletecompletions)

## Enumeration members

### Invoke

•  **Invoke**:  = 0

*Defined in [index.d.ts:4135](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4135)*

Completion was triggered normally.

___

### TriggerCharacter

•  **TriggerCharacter**:  = 1

*Defined in [index.d.ts:4139](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4139)*

Completion was triggered by a trigger character.

___

### TriggerForIncompleteCompletions

•  **TriggerForIncompleteCompletions**:  = 2

*Defined in [index.d.ts:4143](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4143)*

Completion was re-triggered as current completion list is incomplete
