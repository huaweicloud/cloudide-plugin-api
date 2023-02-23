[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SignatureHelpContext

# Interface: SignatureHelpContext

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SignatureHelpContext

Additional information about the context in which a
[`SignatureHelpProvider`](#SignatureHelpProvider.provideSignatureHelp) was triggered.

## Table of contents

### Properties

- [activeSignatureHelp](cloudide_plugin_.SignatureHelpContext.md#activesignaturehelp)
- [isRetrigger](cloudide_plugin_.SignatureHelpContext.md#isretrigger)
- [triggerCharacter](cloudide_plugin_.SignatureHelpContext.md#triggercharacter)
- [triggerKind](cloudide_plugin_.SignatureHelpContext.md#triggerkind)

## Properties

### activeSignatureHelp

• `Optional` `Readonly` **activeSignatureHelp**: [`SignatureHelp`](../classes/cloudide_plugin_.SignatureHelp.md)

The currently active [`SignatureHelp`](#SignatureHelp).

The `activeSignatureHelp` has its [`SignatureHelp.activeSignature`] field updated based on
the user arrowing through available signatures.

#### Defined in

[index.d.ts:6860](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6860)

___

### isRetrigger

• `Readonly` **isRetrigger**: `boolean`

`true` if signature help was already showing when it was triggered.

Retriggers occur when the signature help is already active and can be caused by actions such as
typing a trigger character, a cursor move, or document content changes.

#### Defined in

[index.d.ts:6852](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6852)

___

### triggerCharacter

• `Optional` `Readonly` **triggerCharacter**: `string`

Character that caused signature help to be triggered.

This is `undefined` when signature help is not triggered by typing, such as when manually invoking
signature help or when moving the cursor.

#### Defined in

[index.d.ts:6844](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6844)

___

### triggerKind

• `Readonly` **triggerKind**: [`SignatureHelpTriggerKind`](../enums/cloudide_plugin_.SignatureHelpTriggerKind.md)

Action that caused signature help to be triggered.

#### Defined in

[index.d.ts:6836](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6836)
