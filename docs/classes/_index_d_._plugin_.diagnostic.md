**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Diagnostic

# Class: Diagnostic

Represents a diagnostic, such as a compiler error or warning. Diagnostic objects
are only valid in the scope of a file.

## Hierarchy

* **Diagnostic**

## Index

### Constructors

* [constructor](_index_d_._plugin_.diagnostic.md#constructor)

### Properties

* [code](_index_d_._plugin_.diagnostic.md#code)
* [message](_index_d_._plugin_.diagnostic.md#message)
* [range](_index_d_._plugin_.diagnostic.md#range)
* [relatedInformation](_index_d_._plugin_.diagnostic.md#relatedinformation)
* [severity](_index_d_._plugin_.diagnostic.md#severity)
* [source](_index_d_._plugin_.diagnostic.md#source)
* [tags](_index_d_._plugin_.diagnostic.md#tags)

## Constructors

### constructor

\+ **new Diagnostic**(`range`: [Range](_index_d_._plugin_.range.md), `message`: string, `severity?`: [DiagnosticSeverity](../enums/_index_d_._plugin_.diagnosticseverity.md)): [Diagnostic](_index_d_._plugin_.diagnostic.md)

*Defined in [index.d.ts:5273](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5273)*

Creates a new diagnostic object.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`range` | [Range](_index_d_._plugin_.range.md) | The range to which this diagnostic applies. |
`message` | string | The human-readable message. |
`severity?` | [DiagnosticSeverity](../enums/_index_d_._plugin_.diagnosticseverity.md) | The severity, default is [error](#DiagnosticSeverity.Error).  |

**Returns:** [Diagnostic](_index_d_._plugin_.diagnostic.md)

## Properties

### code

• `Optional` **code**: string \| number \| { target: [Uri](_index_d_._plugin_.uri.md) ; value: string \| number  }

*Defined in [index.d.ts:5251](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5251)*

A code or identifier for this diagnostic.
Should be used for later processing, e.g. when providing [code actions](#CodeActionContext).

___

### message

•  **message**: string

*Defined in [index.d.ts:5234](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5234)*

The human-readable message.

___

### range

•  **range**: [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:5229](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5229)*

The range to which this diagnostic applies.

___

### relatedInformation

• `Optional` **relatedInformation**: [DiagnosticRelatedInformation](_index_d_._plugin_.diagnosticrelatedinformation.md)[]

*Defined in [index.d.ts:5268](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5268)*

An array of related diagnostic information, e.g. when symbol-names within
a scope collide all definitions can be marked via this property.

___

### severity

•  **severity**: [DiagnosticSeverity](../enums/_index_d_._plugin_.diagnosticseverity.md)

*Defined in [index.d.ts:5239](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5239)*

The severity, default is [error](#DiagnosticSeverity.Error).

___

### source

• `Optional` **source**: string

*Defined in [index.d.ts:5245](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5245)*

A human-readable string describing the source of this
diagnostic, e.g. 'typescript' or 'super lint'.

___

### tags

• `Optional` **tags**: [DiagnosticTag](../enums/_index_d_._plugin_.diagnostictag.md)[]

*Defined in [index.d.ts:5273](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5273)*

Additional metadata about the diagnostic.
