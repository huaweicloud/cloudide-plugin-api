[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SignatureHelpTriggerKind

# Enumeration: SignatureHelpTriggerKind

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SignatureHelpTriggerKind

How a [`SignatureHelpProvider`](#SignatureHelpProvider) was triggered.

## Table of contents

### Enumeration Members

- [ContentChange](cloudide_plugin_.SignatureHelpTriggerKind.md#contentchange)
- [Invoke](cloudide_plugin_.SignatureHelpTriggerKind.md#invoke)
- [TriggerCharacter](cloudide_plugin_.SignatureHelpTriggerKind.md#triggercharacter)

## Enumeration Members

### ContentChange

• **ContentChange** = ``3``

Signature help was triggered by the cursor moving or by the document content changing.

#### Defined in

[index.d.ts:6825](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6825)

___

### Invoke

• **Invoke** = ``1``

Signature help was invoked manually by the user or by a command.

#### Defined in

[index.d.ts:6815](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6815)

___

### TriggerCharacter

• **TriggerCharacter** = ``2``

Signature help was triggered by a trigger character.

#### Defined in

[index.d.ts:6820](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6820)
