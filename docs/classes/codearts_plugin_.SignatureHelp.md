[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SignatureHelp

# Class: SignatureHelp

["@codearts/plugin"](../modules/_codearts_plugin_.md).SignatureHelp

Signature help represents the signature of something
callable. There can be multiple signatures but only one
active and only one active parameter.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.SignatureHelp.md#constructor)

### Properties

- [activeParameter](codearts_plugin_.SignatureHelp.md#activeparameter)
- [activeSignature](codearts_plugin_.SignatureHelp.md#activesignature)
- [signatures](codearts_plugin_.SignatureHelp.md#signatures)

## Constructors

### constructor

• **new SignatureHelp**()

## Properties

### activeParameter

• **activeParameter**: `number`

The active parameter of the active signature.

#### Defined in

[index.d.ts:4120](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4120)

___

### activeSignature

• **activeSignature**: `number`

The active signature.

#### Defined in

[index.d.ts:4115](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4115)

___

### signatures

• **signatures**: [`SignatureInformation`](codearts_plugin_.SignatureInformation.md)[]

One or more signatures.

#### Defined in

[index.d.ts:4110](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L4110)
