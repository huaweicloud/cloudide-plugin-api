**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SignatureHelpContext

# Interface: SignatureHelpContext

Additional information about the context in which a
[`SignatureHelpProvider`](#SignatureHelpProvider.provideSignatureHelp) was triggered.

## Hierarchy

* **SignatureHelpContext**

## Index

### Properties

* [activeSignatureHelp](_index_d_._plugin_.signaturehelpcontext.md#activesignaturehelp)
* [isRetrigger](_index_d_._plugin_.signaturehelpcontext.md#isretrigger)
* [triggerCharacter](_index_d_._plugin_.signaturehelpcontext.md#triggercharacter)
* [triggerKind](_index_d_._plugin_.signaturehelpcontext.md#triggerkind)

## Properties

### activeSignatureHelp

• `Optional` `Readonly` **activeSignatureHelp**: [SignatureHelp](../classes/_index_d_._plugin_.signaturehelp.md)

*Defined in [index.d.ts:3641](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3641)*

The currently active [`SignatureHelp`](#SignatureHelp).

The `activeSignatureHelp` has its [`SignatureHelp.activeSignature`] field updated based on
the user arrowing through available signatures.

___

### isRetrigger

• `Readonly` **isRetrigger**: boolean

*Defined in [index.d.ts:3633](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3633)*

`true` if signature help was already showing when it was triggered.

Retriggers occur when the signature help is already active and can be caused by actions such as
typing a trigger character, a cursor move, or document content changes.

___

### triggerCharacter

• `Optional` `Readonly` **triggerCharacter**: string

*Defined in [index.d.ts:3625](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3625)*

Character that caused signature help to be triggered.

This is `undefined` when signature help is not triggered by typing, such as when manually invoking
signature help or when moving the cursor.

___

### triggerKind

• `Readonly` **triggerKind**: [SignatureHelpTriggerKind](../enums/_index_d_._plugin_.signaturehelptriggerkind.md)

*Defined in [index.d.ts:3617](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3617)*

Action that caused signature help to be triggered.
