[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DiagnosticRelatedInformation

# Class: DiagnosticRelatedInformation

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DiagnosticRelatedInformation

Represents a related message and source code location for a diagnostic. This should be
used to point to code locations that cause or related to a diagnostics, e.g when duplicating
a symbol in a scope.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.DiagnosticRelatedInformation.md#constructor)

### Properties

- [location](cloudide_plugin_.DiagnosticRelatedInformation.md#location)
- [message](cloudide_plugin_.DiagnosticRelatedInformation.md#message)

## Constructors

### constructor

• **new DiagnosticRelatedInformation**(`location`, `message`)

Creates a new related diagnostic information object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `location` | [`Location`](cloudide_plugin_.Location.md) | The location. |
| `message` | `string` | The message. |

#### Defined in

[index.d.ts:7765](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7765)

## Properties

### location

• **location**: [`Location`](cloudide_plugin_.Location.md)

The location of this related diagnostic information.

#### Defined in

[index.d.ts:7752](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7752)

___

### message

• **message**: `string`

The message of this related diagnostic information.

#### Defined in

[index.d.ts:7757](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7757)
