[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Diagnostic

# Class: Diagnostic

["@codearts/plugin"](../modules/_codearts_plugin_.md).Diagnostic

Represents a diagnostic, such as a compiler error or warning. Diagnostic objects
are only valid in the scope of a file.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.Diagnostic.md#constructor)

### Properties

- [code](codearts_plugin_.Diagnostic.md#code)
- [message](codearts_plugin_.Diagnostic.md#message)
- [range](codearts_plugin_.Diagnostic.md#range)
- [relatedInformation](codearts_plugin_.Diagnostic.md#relatedinformation)
- [severity](codearts_plugin_.Diagnostic.md#severity)
- [source](codearts_plugin_.Diagnostic.md#source)
- [tags](codearts_plugin_.Diagnostic.md#tags)

## Constructors

### constructor

• **new Diagnostic**(`range`, `message`, `severity?`)

Creates a new diagnostic object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) | The range to which this diagnostic applies. |
| `message` | `string` | The human-readable message. |
| `severity?` | [`DiagnosticSeverity`](../enums/codearts_plugin_.DiagnosticSeverity.md) | The severity, default is [error](../enums/codearts_plugin_.DiagnosticSeverity.md#error). |

#### Defined in

[index.d.ts:6046](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6046)

## Properties

### code

• `Optional` **code**: `string` \| `number` \| { `target`: [`Uri`](codearts_plugin_.Uri.md) ; `value`: `string` \| `number`  }

A code or identifier for this diagnostic.
Should be used for later processing, e.g. when providing [code actions](../interfaces/codearts_plugin_.CodeActionContext.md).

#### Defined in

[index.d.ts:6015](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6015)

___

### message

• **message**: `string`

The human-readable message.

#### Defined in

[index.d.ts:5998](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5998)

___

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

The range to which this diagnostic applies.

#### Defined in

[index.d.ts:5993](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5993)

___

### relatedInformation

• `Optional` **relatedInformation**: [`DiagnosticRelatedInformation`](codearts_plugin_.DiagnosticRelatedInformation.md)[]

An array of related diagnostic information, e.g. when symbol-names within
a scope collide all definitions can be marked via this property.

#### Defined in

[index.d.ts:6032](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6032)

___

### severity

• **severity**: [`DiagnosticSeverity`](../enums/codearts_plugin_.DiagnosticSeverity.md)

The severity, default is [error](../enums/codearts_plugin_.DiagnosticSeverity.md#error).

#### Defined in

[index.d.ts:6003](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6003)

___

### source

• `Optional` **source**: `string`

A human-readable string describing the source of this
diagnostic, e.g. 'typescript' or 'super lint'.

#### Defined in

[index.d.ts:6009](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6009)

___

### tags

• `Optional` **tags**: [`DiagnosticTag`](../enums/codearts_plugin_.DiagnosticTag.md)[]

Additional metadata about the diagnostic.

#### Defined in

[index.d.ts:6037](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6037)
