[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SignatureHelpProviderMetadata

# Interface: SignatureHelpProviderMetadata

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SignatureHelpProviderMetadata

Metadata about a registered [`SignatureHelpProvider`](#SignatureHelpProvider).

## Table of contents

### Properties

- [retriggerCharacters](cloudide_plugin_.SignatureHelpProviderMetadata.md#retriggercharacters)
- [triggerCharacters](cloudide_plugin_.SignatureHelpProviderMetadata.md#triggercharacters)

## Properties

### retriggerCharacters

• `Readonly` **retriggerCharacters**: readonly `string`[]

List of characters that re-trigger signature help.

These trigger characters are only active when signature help is already showing. All trigger characters
are also counted as re-trigger characters.

#### Defined in

[index.d.ts:6898](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6898)

___

### triggerCharacters

• `Readonly` **triggerCharacters**: readonly `string`[]

List of characters that trigger signature help.

#### Defined in

[index.d.ts:6890](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6890)
