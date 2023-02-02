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

[index.d.ts:6000](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L6000)

## Properties

### code

• `Optional` **code**: `string` \| `number` \| { `target`: [`Uri`](codearts_plugin_.Uri.md) ; `value`: `string` \| `number`  }

A code or identifier for this diagnostic.
Should be used for later processing, e.g. when providing [code actions](../interfaces/codearts_plugin_.CodeActionContext.md).

#### Defined in

[index.d.ts:5969](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5969)

___

### message

• **message**: `string`

The human-readable message.

#### Defined in

[index.d.ts:5952](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5952)

___

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

The range to which this diagnostic applies.

#### Defined in

[index.d.ts:5947](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5947)

___

### relatedInformation

• `Optional` **relatedInformation**: [`DiagnosticRelatedInformation`](codearts_plugin_.DiagnosticRelatedInformation.md)[]

An array of related diagnostic information, e.g. when symbol-names within
a scope collide all definitions can be marked via this property.

#### Defined in

[index.d.ts:5986](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5986)

___

### severity

• **severity**: [`DiagnosticSeverity`](../enums/codearts_plugin_.DiagnosticSeverity.md)

The severity, default is [error](../enums/codearts_plugin_.DiagnosticSeverity.md#error).

#### Defined in

[index.d.ts:5957](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5957)

___

### source

• `Optional` **source**: `string`

A human-readable string describing the source of this
diagnostic, e.g. 'typescript' or 'super lint'.

#### Defined in

[index.d.ts:5963](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5963)

___

### tags

• `Optional` **tags**: [`DiagnosticTag`](../enums/codearts_plugin_.DiagnosticTag.md)[]

Additional metadata about the diagnostic.

#### Defined in

[index.d.ts:5991](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5991)
