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

*Defined in [index.d.ts:4891](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4891)*

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

*Defined in [index.d.ts:4886](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4886)*

The location of this related diagnostic information.

___

### message

•  **message**: string

*Defined in [index.d.ts:4891](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4891)*

The message of this related diagnostic information.
