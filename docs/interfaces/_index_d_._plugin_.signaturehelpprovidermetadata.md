**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SignatureHelpProviderMetadata

# Interface: SignatureHelpProviderMetadata

Metadata about a registered [`SignatureHelpProvider`](#SignatureHelpProvider).

## Hierarchy

* **SignatureHelpProviderMetadata**

## Index

### Properties

* [retriggerCharacters](_index_d_._plugin_.signaturehelpprovidermetadata.md#retriggercharacters)
* [triggerCharacters](_index_d_._plugin_.signaturehelpprovidermetadata.md#triggercharacters)

## Properties

### retriggerCharacters

• `Readonly` **retriggerCharacters**: ReadonlyArray\<string>

*Defined in [index.d.ts:3679](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3679)*

List of characters that re-trigger signature help.

These trigger characters are only active when signature help is already showing. All trigger characters
are also counted as re-trigger characters.

___

### triggerCharacters

• `Readonly` **triggerCharacters**: ReadonlyArray\<string>

*Defined in [index.d.ts:3671](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3671)*

List of characters that trigger signature help.
