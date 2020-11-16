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

*Defined in [index.d.ts:3586](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3586)*

The active parameter of the active signature.

___

### activeSignature

•  **activeSignature**: number

*Defined in [index.d.ts:3581](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3581)*

The active signature.

___

### signatures

•  **signatures**: [SignatureInformation](_index_d_._plugin_.signatureinformation.md)[]

*Defined in [index.d.ts:3576](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3576)*

One or more signatures.
