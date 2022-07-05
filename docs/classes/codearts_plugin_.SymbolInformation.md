[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SymbolInformation

# Class: SymbolInformation

["@codearts/plugin"](../modules/_codearts_plugin_.md).SymbolInformation

## Table of contents

### Constructors

- [constructor](codearts_plugin_.SymbolInformation.md#constructor)

### Properties

- [containerName](codearts_plugin_.SymbolInformation.md#containername)
- [kind](codearts_plugin_.SymbolInformation.md#kind)
- [location](codearts_plugin_.SymbolInformation.md#location)
- [name](codearts_plugin_.SymbolInformation.md#name)
- [tags](codearts_plugin_.SymbolInformation.md#tags)

## Constructors

### constructor

• **new SymbolInformation**(`name`, `kind`, `containerName`, `location`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` |  |
| `kind` | [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md) |  |
| `containerName` | `string` |  |
| `location` | [`Location`](codearts_plugin_.Location.md) |  |

#### Defined in

[index.d.ts:3202](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L3202)

• **new SymbolInformation**(`name`, `kind`, `range`, `uri?`, `containerName?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` |  |
| `kind` | [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md) |  |
| `range` | [`Range`](codearts_plugin_.Range.md) |  |
| `uri?` | [`Uri`](codearts_plugin_.Uri.md) |  |
| `containerName?` | `string` |  |

#### Defined in

[index.d.ts:3215](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L3215)

## Properties

### containerName

• **containerName**: `string`

#### Defined in

[index.d.ts:3177](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L3177)

___

### kind

• **kind**: [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md)

#### Defined in

[index.d.ts:3182](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L3182)

___

### location

• **location**: [`Location`](codearts_plugin_.Location.md)

#### Defined in

[index.d.ts:3192](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L3192)

___

### name

• **name**: `string`

#### Defined in

[index.d.ts:3172](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L3172)

___

### tags

• `Optional` **tags**: readonly [`Deprecated`](../enums/codearts_plugin_.SymbolTag.md#deprecated)[]

#### Defined in

[index.d.ts:3187](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L3187)
