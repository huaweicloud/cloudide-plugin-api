[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SignatureHelp

# Class: SignatureHelp

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SignatureHelp

Signature help represents the signature of something
callable. There can be multiple signatures but only one
active and only one active parameter.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.SignatureHelp.md#constructor)

### Properties

- [activeParameter](cloudide_plugin_.SignatureHelp.md#activeparameter)
- [activeSignature](cloudide_plugin_.SignatureHelp.md#activesignature)
- [signatures](cloudide_plugin_.SignatureHelp.md#signatures)

## Constructors

### constructor

• **new SignatureHelp**()

## Properties

### activeParameter

• **activeParameter**: `number`

The active parameter of the active signature.

#### Defined in

[index.d.ts:6805](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6805)

___

### activeSignature

• **activeSignature**: `number`

The active signature.

#### Defined in

[index.d.ts:6800](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6800)

___

### signatures

• **signatures**: [`SignatureInformation`](cloudide_plugin_.SignatureInformation.md)[]

One or more signatures.

#### Defined in

[index.d.ts:6795](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6795)
