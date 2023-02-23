[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Diagnostic

# Class: Diagnostic

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Diagnostic

Represents a diagnostic, such as a compiler error or warning. Diagnostic objects
are only valid in the scope of a file.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.Diagnostic.md#constructor)

### Properties

- [code](cloudide_plugin_.Diagnostic.md#code)
- [message](cloudide_plugin_.Diagnostic.md#message)
- [range](cloudide_plugin_.Diagnostic.md#range)
- [relatedInformation](cloudide_plugin_.Diagnostic.md#relatedinformation)
- [severity](cloudide_plugin_.Diagnostic.md#severity)
- [source](cloudide_plugin_.Diagnostic.md#source)
- [tags](cloudide_plugin_.Diagnostic.md#tags)

## Constructors

### constructor

• **new Diagnostic**(`range`, `message`, `severity?`)

Creates a new diagnostic object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](cloudide_plugin_.Range.md) | The range to which this diagnostic applies. |
| `message` | `string` | The human-readable message. |
| `severity?` | [`DiagnosticSeverity`](../enums/cloudide_plugin_.DiagnosticSeverity.md) | The severity, default is [error](#DiagnosticSeverity.Error). |

#### Defined in

[index.d.ts:7843](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7843)

## Properties

### code

• `Optional` **code**: `string` \| `number`

A code or identifier for this diagnostics. Will not be surfaced
to the user, but should be used for later processing, e.g. when
providing [code actions](#CodeActionContext).

#### Defined in

[index.d.ts:7823](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7823)

___

### message

• **message**: `string`

The human-readable message.

#### Defined in

[index.d.ts:7805](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7805)

___

### range

• **range**: [`Range`](cloudide_plugin_.Range.md)

The range to which this diagnostic applies.

#### Defined in

[index.d.ts:7800](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7800)

___

### relatedInformation

• `Optional` **relatedInformation**: [`DiagnosticRelatedInformation`](cloudide_plugin_.DiagnosticRelatedInformation.md)[]

An array of related diagnostic information, e.g. when symbol-names within
a scope collide all definitions can be marked via this property.

#### Defined in

[index.d.ts:7829](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7829)

___

### severity

• **severity**: [`DiagnosticSeverity`](../enums/cloudide_plugin_.DiagnosticSeverity.md)

The severity, default is [error](#DiagnosticSeverity.Error).

#### Defined in

[index.d.ts:7810](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7810)

___

### source

• `Optional` **source**: `string`

A human-readable string describing the source of this
diagnostic, e.g. 'typescript' or 'super lint'.

#### Defined in

[index.d.ts:7816](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7816)

___

### tags

• `Optional` **tags**: [`DiagnosticTag`](../enums/cloudide_plugin_.DiagnosticTag.md)[]

Additional metadata about the diagnostic.

#### Defined in

[index.d.ts:7834](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7834)
