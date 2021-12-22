**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DiagnosticRelatedInformation

# Class: DiagnosticRelatedInformation

Represents a related message and source code location for a diagnostic. This should be
used to point to code locations that cause or related to a diagnostics, e.g. when duplicating
a symbol in a scope.

## Hierarchy

* **DiagnosticRelatedInformation**

## Index

### Constructors

* [constructor](_index_d_._plugin_.diagnosticrelatedinformation.md#constructor)

### Properties

* [location](_index_d_._plugin_.diagnosticrelatedinformation.md#location)
* [message](_index_d_._plugin_.diagnosticrelatedinformation.md#message)

## Constructors

### constructor

\+ **new DiagnosticRelatedInformation**(`location`: [Location](_index_d_._plugin_.location.md), `message`: string): [DiagnosticRelatedInformation](_index_d_._plugin_.diagnosticrelatedinformation.md)

*Defined in [index.d.ts:5188](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5188)*

Creates a new related diagnostic information object.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`location` | [Location](_index_d_._plugin_.location.md) | The location. |
`message` | string | The message.  |

**Returns:** [DiagnosticRelatedInformation](_index_d_._plugin_.diagnosticrelatedinformation.md)

## Properties

### location

•  **location**: [Location](_index_d_._plugin_.location.md)

*Defined in [index.d.ts:5183](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5183)*

The location of this related diagnostic information.

___

### message

•  **message**: string

*Defined in [index.d.ts:5188](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L5188)*

The message of this related diagnostic information.
