[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DocumentSymbol

# Class: DocumentSymbol

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DocumentSymbol

Represents programming constructs like variables, classes, interfaces etc. that appear in a document. Document
symbols can be hierarchical and they have two ranges: one that encloses its definition and one that points to
its most interesting range, e.g. the range of an identifier.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.DocumentSymbol.md#constructor)

### Properties

- [children](cloudide_plugin_.DocumentSymbol.md#children)
- [detail](cloudide_plugin_.DocumentSymbol.md#detail)
- [kind](cloudide_plugin_.DocumentSymbol.md#kind)
- [name](cloudide_plugin_.DocumentSymbol.md#name)
- [range](cloudide_plugin_.DocumentSymbol.md#range)
- [selectionRange](cloudide_plugin_.DocumentSymbol.md#selectionrange)
- [tags](cloudide_plugin_.DocumentSymbol.md#tags)

## Constructors

### constructor

• **new DocumentSymbol**(`name`, `detail`, `kind`, `range`, `selectionRange`)

Creates a new document symbol.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the symbol. |
| `detail` | `string` | Details for the symbol. |
| `kind` | [`SymbolKind`](../enums/cloudide_plugin_.SymbolKind.md) | The kind of the symbol. |
| `range` | [`Range`](cloudide_plugin_.Range.md) | The full range of the symbol. |
| `selectionRange` | [`Range`](cloudide_plugin_.Range.md) | The range that should be reveal. |

#### Defined in

[index.d.ts:7085](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7085)

## Properties

### children

• **children**: [`DocumentSymbol`](cloudide_plugin_.DocumentSymbol.md)[]

Children of this symbol, e.g. properties of a class.

#### Defined in

[index.d.ts:7074](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7074)

___

### detail

• **detail**: `string`

More detail for this symbol, e.g the signature of a function.

#### Defined in

[index.d.ts:7051](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7051)

___

### kind

• **kind**: [`SymbolKind`](../enums/cloudide_plugin_.SymbolKind.md)

The kind of this symbol.

#### Defined in

[index.d.ts:7056](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7056)

___

### name

• **name**: `string`

The name of this symbol.

#### Defined in

[index.d.ts:7046](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7046)

___

### range

• **range**: [`Range`](cloudide_plugin_.Range.md)

The range enclosing this symbol not including leading/trailing whitespace but everything else, e.g comments and code.

#### Defined in

[index.d.ts:7063](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7063)

___

### selectionRange

• **selectionRange**: [`Range`](cloudide_plugin_.Range.md)

The range that should be selected and reveal when this symbol is being picked, e.g the name of a function.
Must be contained by the [`range`](#DocumentSymbol.range).

#### Defined in

[index.d.ts:7069](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7069)

___

### tags

• `Optional` **tags**: readonly [`Deprecated`](../enums/cloudide_plugin_.SymbolTag.md#deprecated)[]

#### Defined in

[index.d.ts:7058](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7058)
