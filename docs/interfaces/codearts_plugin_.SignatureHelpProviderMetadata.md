[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SignatureHelpProviderMetadata

# Interface: SignatureHelpProviderMetadata

["@codearts/plugin"](../modules/_codearts_plugin_.md).SignatureHelpProviderMetadata

Metadata about a registered [`SignatureHelpProvider`](codearts_plugin_.SignatureHelpProvider.md).

## Table of contents

### Properties

- [retriggerCharacters](codearts_plugin_.SignatureHelpProviderMetadata.md#retriggercharacters)
- [triggerCharacters](codearts_plugin_.SignatureHelpProviderMetadata.md#triggercharacters)

## Properties

### retriggerCharacters

• `Readonly` **retriggerCharacters**: readonly `string`[]

List of characters that re-trigger signature help.

These trigger characters are only active when signature help is already showing. All trigger characters
are also counted as re-trigger characters.

#### Defined in

[index.d.ts:4213](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4213)

___

### triggerCharacters

• `Readonly` **triggerCharacters**: readonly `string`[]

List of characters that trigger signature help.

#### Defined in

[index.d.ts:4205](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4205)
