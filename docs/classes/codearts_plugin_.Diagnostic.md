[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Diagnostic

# Class: Diagnostic

["@codearts/plugin"](../modules/_codearts_plugin_.md).Diagnostic

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) |  |
| `message` | `string` |  |
| `severity?` | [`DiagnosticSeverity`](../enums/codearts_plugin_.DiagnosticSeverity.md) |  |

#### Defined in

[index.d.ts:5980](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L5980)

## Properties

### code

• `Optional` **code**: `string` \| `number` \| { `target`: [`Uri`](codearts_plugin_.Uri.md) ; `value`: `string` \| `number`  }

#### Defined in

[index.d.ts:5949](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L5949)

___

### message

• **message**: `string`

#### Defined in

[index.d.ts:5932](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L5932)

___

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

#### Defined in

[index.d.ts:5927](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L5927)

___

### relatedInformation

• `Optional` **relatedInformation**: [`DiagnosticRelatedInformation`](codearts_plugin_.DiagnosticRelatedInformation.md)[]

#### Defined in

[index.d.ts:5966](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L5966)

___

### severity

• **severity**: [`DiagnosticSeverity`](../enums/codearts_plugin_.DiagnosticSeverity.md)

#### Defined in

[index.d.ts:5937](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L5937)

___

### source

• `Optional` **source**: `string`

#### Defined in

[index.d.ts:5943](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L5943)

___

### tags

• `Optional` **tags**: [`DiagnosticTag`](../enums/codearts_plugin_.DiagnosticTag.md)[]

#### Defined in

[index.d.ts:5971](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L5971)
