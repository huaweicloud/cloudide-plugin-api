[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SignatureHelpTriggerKind

# Enumeration: SignatureHelpTriggerKind

["@codearts/plugin"](../modules/_codearts_plugin_.md).SignatureHelpTriggerKind

How a [`SignatureHelpProvider`](../interfaces/codearts_plugin_.SignatureHelpProvider.md) was triggered.

## Table of contents

### Enumeration Members

- [ContentChange](codearts_plugin_.SignatureHelpTriggerKind.md#contentchange)
- [Invoke](codearts_plugin_.SignatureHelpTriggerKind.md#invoke)
- [TriggerCharacter](codearts_plugin_.SignatureHelpTriggerKind.md#triggercharacter)

## Enumeration Members

### ContentChange

• **ContentChange** = ``3``

Signature help was triggered by the cursor moving or by the document content changing.

#### Defined in

[index.d.ts:4102](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L4102)

___

### Invoke

• **Invoke** = ``1``

Signature help was invoked manually by the user or by a command.

#### Defined in

[index.d.ts:4092](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L4092)

___

### TriggerCharacter

• **TriggerCharacter** = ``2``

Signature help was triggered by a trigger character.

#### Defined in

[index.d.ts:4097](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L4097)
