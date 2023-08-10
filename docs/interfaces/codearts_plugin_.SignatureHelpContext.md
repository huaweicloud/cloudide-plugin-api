[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SignatureHelpContext

# Interface: SignatureHelpContext

["@codearts/plugin"](../modules/_codearts_plugin_.md).SignatureHelpContext

Additional information about the context in which a
[`SignatureHelpProvider`](codearts_plugin_.SignatureHelpProvider.md#providesignaturehelp) was triggered.

## Table of contents

### Properties

- [activeSignatureHelp](codearts_plugin_.SignatureHelpContext.md#activesignaturehelp)
- [isRetrigger](codearts_plugin_.SignatureHelpContext.md#isretrigger)
- [triggerCharacter](codearts_plugin_.SignatureHelpContext.md#triggercharacter)
- [triggerKind](codearts_plugin_.SignatureHelpContext.md#triggerkind)

## Properties

### activeSignatureHelp

• `Readonly` **activeSignatureHelp**: `undefined` \| [`SignatureHelp`](../classes/codearts_plugin_.SignatureHelp.md)

The currently active [`SignatureHelp`](../classes/codearts_plugin_.SignatureHelp.md).

The `activeSignatureHelp` has its [`SignatureHelp.activeSignature`] field updated based on
the user arrowing through available signatures.

#### Defined in

[index.d.ts:4175](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4175)

___

### isRetrigger

• `Readonly` **isRetrigger**: `boolean`

`true` if signature help was already showing when it was triggered.

Retriggers occur when the signature help is already active and can be caused by actions such as
typing a trigger character, a cursor move, or document content changes.

#### Defined in

[index.d.ts:4167](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4167)

___

### triggerCharacter

• `Readonly` **triggerCharacter**: `undefined` \| `string`

Character that caused signature help to be triggered.

This is `undefined` when signature help is not triggered by typing, such as when manually invoking
signature help or when moving the cursor.

#### Defined in

[index.d.ts:4159](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4159)

___

### triggerKind

• `Readonly` **triggerKind**: [`SignatureHelpTriggerKind`](../enums/codearts_plugin_.SignatureHelpTriggerKind.md)

Action that caused signature help to be triggered.

#### Defined in

[index.d.ts:4151](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4151)
