[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentSymbol

# Class: DocumentSymbol

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentSymbol

## Table of contents

### Constructors

- [constructor](codearts_plugin_.DocumentSymbol.md#constructor)

### Properties

- [children](codearts_plugin_.DocumentSymbol.md#children)
- [detail](codearts_plugin_.DocumentSymbol.md#detail)
- [kind](codearts_plugin_.DocumentSymbol.md#kind)
- [name](codearts_plugin_.DocumentSymbol.md#name)
- [range](codearts_plugin_.DocumentSymbol.md#range)
- [selectionRange](codearts_plugin_.DocumentSymbol.md#selectionrange)
- [tags](codearts_plugin_.DocumentSymbol.md#tags)

## Constructors

### constructor

• **new DocumentSymbol**(`name`, `detail`, `kind`, `range`, `selectionRange`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` |  |
| `detail` | `string` |  |
| `kind` | [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md) |  |
| `range` | [`Range`](codearts_plugin_.Range.md) |  |
| `selectionRange` | [`Range`](codearts_plugin_.Range.md) |  |

#### Defined in

[index.d.ts:3270](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3270)

## Properties

### children

• **children**: [`DocumentSymbol`](codearts_plugin_.DocumentSymbol.md)[]

#### Defined in

[index.d.ts:3259](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3259)

___

### detail

• **detail**: `string`

#### Defined in

[index.d.ts:3233](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3233)

___

### kind

• **kind**: [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md)

#### Defined in

[index.d.ts:3238](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3238)

___

### name

• **name**: `string`

#### Defined in

[index.d.ts:3228](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3228)

___

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

#### Defined in

[index.d.ts:3248](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3248)

___

### selectionRange

• **selectionRange**: [`Range`](codearts_plugin_.Range.md)

#### Defined in

[index.d.ts:3254](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3254)

___

### tags

• `Optional` **tags**: readonly [`Deprecated`](../enums/codearts_plugin_.SymbolTag.md#deprecated)[]

#### Defined in

[index.d.ts:3243](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3243)
