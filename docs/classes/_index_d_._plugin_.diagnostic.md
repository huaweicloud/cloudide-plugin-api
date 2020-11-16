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

*Defined in [index.d.ts:4979](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4979)*

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

*Defined in [index.d.ts:4957](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4957)*

A code or identifier for this diagnostic.
Should be used for later processing, e.g. when providing [code actions](#CodeActionContext).

___

### message

•  **message**: string

*Defined in [index.d.ts:4940](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4940)*

The human-readable message.

___

### range

•  **range**: [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:4935](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4935)*

The range to which this diagnostic applies.

___

### relatedInformation

• `Optional` **relatedInformation**: [DiagnosticRelatedInformation](_index_d_._plugin_.diagnosticrelatedinformation.md)[]

*Defined in [index.d.ts:4974](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4974)*

An array of related diagnostic information, e.g. when symbol-names within
a scope collide all definitions can be marked via this property.

___

### severity

•  **severity**: [DiagnosticSeverity](../enums/_index_d_._plugin_.diagnosticseverity.md)

*Defined in [index.d.ts:4945](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4945)*

The severity, default is [error](#DiagnosticSeverity.Error).

___

### source

• `Optional` **source**: string

*Defined in [index.d.ts:4951](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4951)*

A human-readable string describing the source of this
diagnostic, e.g. 'typescript' or 'super lint'.

___

### tags

• `Optional` **tags**: [DiagnosticTag](../enums/_index_d_._plugin_.diagnostictag.md)[]

*Defined in [index.d.ts:4979](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4979)*

Additional metadata about the diagnostic.
