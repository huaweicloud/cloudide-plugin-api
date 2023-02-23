[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CompletionContext

# Interface: CompletionContext

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CompletionContext

Contains additional information about the context in which
[completion provider](#CompletionItemProvider.provideCompletionItems) is triggered.

## Table of contents

### Properties

- [triggerCharacter](cloudide_plugin_.CompletionContext.md#triggercharacter)
- [triggerKind](cloudide_plugin_.CompletionContext.md#triggerkind)

## Properties

### triggerCharacter

• `Optional` `Readonly` **triggerCharacter**: `string`

Character that triggered the completion item provider.

`undefined` if provider was not triggered by a character.

The trigger character is already in the document when the completion provider is triggered.

#### Defined in

[index.d.ts:6936](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6936)

___

### triggerKind

• `Readonly` **triggerKind**: [`CompletionTriggerKind`](../enums/cloudide_plugin_.CompletionTriggerKind.md)

How the completion was triggered.

#### Defined in

[index.d.ts:6927](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6927)
