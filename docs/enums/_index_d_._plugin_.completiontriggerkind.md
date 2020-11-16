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

*Defined in [index.d.ts:3898](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3898)*

Completion was triggered normally.

___

### TriggerCharacter

•  **TriggerCharacter**:  = 1

*Defined in [index.d.ts:3902](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3902)*

Completion was triggered by a trigger character.

___

### TriggerForIncompleteCompletions

•  **TriggerForIncompleteCompletions**:  = 2

*Defined in [index.d.ts:3906](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3906)*

Completion was re-triggered as current completion list is incomplete
