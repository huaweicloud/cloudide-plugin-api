**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SignatureHelpTriggerKind

# Enumeration: SignatureHelpTriggerKind

How a [`SignatureHelpProvider`](#SignatureHelpProvider) was triggered.

## Index

### Enumeration members

* [ContentChange](_index_d_._plugin_.signaturehelptriggerkind.md#contentchange)
* [Invoke](_index_d_._plugin_.signaturehelptriggerkind.md#invoke)
* [TriggerCharacter](_index_d_._plugin_.signaturehelptriggerkind.md#triggercharacter)

## Enumeration members

### ContentChange

•  **ContentChange**:  = 3

*Defined in [index.d.ts:3606](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3606)*

Signature help was triggered by the cursor moving or by the document content changing.

___

### Invoke

•  **Invoke**:  = 1

*Defined in [index.d.ts:3596](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3596)*

Signature help was invoked manually by the user or by a command.

___

### TriggerCharacter

•  **TriggerCharacter**:  = 2

*Defined in [index.d.ts:3601](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3601)*

Signature help was triggered by a trigger character.
