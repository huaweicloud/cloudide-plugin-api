**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SignatureHelp

# Class: SignatureHelp

Signature help represents the signature of something
callable. There can be multiple signatures but only one
active and only one active parameter.

## Hierarchy

* **SignatureHelp**

## Index

### Properties

* [activeParameter](_index_d_._plugin_.signaturehelp.md#activeparameter)
* [activeSignature](_index_d_._plugin_.signaturehelp.md#activesignature)
* [signatures](_index_d_._plugin_.signaturehelp.md#signatures)

## Properties

### activeParameter

•  **activeParameter**: number

*Defined in [index.d.ts:3813](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3813)*

The active parameter of the active signature.

___

### activeSignature

•  **activeSignature**: number

*Defined in [index.d.ts:3808](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3808)*

The active signature.

___

### signatures

•  **signatures**: [SignatureInformation](_index_d_._plugin_.signatureinformation.md)[]

*Defined in [index.d.ts:3803](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3803)*

One or more signatures.
