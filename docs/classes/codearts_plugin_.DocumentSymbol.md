[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentSymbol

# Class: DocumentSymbol

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentSymbol

Represents programming constructs like variables, classes, interfaces etc. that appear in a document. Document
symbols can be hierarchical and they have two ranges: one that encloses its definition and one that points to
its most interesting range, e.g. the range of an identifier.

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

Creates a new document symbol.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the symbol. |
| `detail` | `string` | Details for the symbol. |
| `kind` | [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md) | The kind of the symbol. |
| `range` | [`Range`](codearts_plugin_.Range.md) | The full range of the symbol. |
| `selectionRange` | [`Range`](codearts_plugin_.Range.md) | The range that should be reveal. |

#### Defined in

[index.d.ts:3270](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L3270)

## Properties

### children

• **children**: [`DocumentSymbol`](codearts_plugin_.DocumentSymbol.md)[]

Children of this symbol, e.g. properties of a class.

#### Defined in

[index.d.ts:3259](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L3259)

___

### detail

• **detail**: `string`

More detail for this symbol, e.g. the signature of a function.

#### Defined in

[index.d.ts:3233](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L3233)

___

### kind

• **kind**: [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md)

The kind of this symbol.

#### Defined in

[index.d.ts:3238](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L3238)

___

### name

• **name**: `string`

The name of this symbol.

#### Defined in

[index.d.ts:3228](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L3228)

___

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

The range enclosing this symbol not including leading/trailing whitespace but everything else, e.g. comments and code.

#### Defined in

[index.d.ts:3248](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L3248)

___

### selectionRange

• **selectionRange**: [`Range`](codearts_plugin_.Range.md)

The range that should be selected and reveal when this symbol is being picked, e.g. the name of a function.
Must be contained by the [`range`](codearts_plugin_.DocumentSymbol.md#range).

#### Defined in

[index.d.ts:3254](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L3254)

___

### tags

• `Optional` **tags**: readonly [`Deprecated`](../enums/codearts_plugin_.SymbolTag.md#deprecated)[]

Tags for this symbol.

#### Defined in

[index.d.ts:3243](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L3243)
