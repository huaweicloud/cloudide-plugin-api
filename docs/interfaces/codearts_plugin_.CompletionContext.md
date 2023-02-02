[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CompletionContext

# Interface: CompletionContext

["@codearts/plugin"](../modules/_codearts_plugin_.md).CompletionContext

Contains additional information about the context in which
[completion provider](codearts_plugin_.CompletionItemProvider.md#providecompletionitems) is triggered.

## Table of contents

### Properties

- [triggerCharacter](codearts_plugin_.CompletionContext.md#triggercharacter)
- [triggerKind](codearts_plugin_.CompletionContext.md#triggerkind)

## Properties

### triggerCharacter

• `Readonly` **triggerCharacter**: `undefined` \| `string`

Character that triggered the completion item provider.

`undefined` if the provider was not triggered by a character.

The trigger character is already in the document when the completion provider is triggered.

#### Defined in

[index.d.ts:4477](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L4477)

___

### triggerKind

• `Readonly` **triggerKind**: [`CompletionTriggerKind`](../enums/codearts_plugin_.CompletionTriggerKind.md)

How the completion was triggered.

#### Defined in

[index.d.ts:4468](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L4468)
