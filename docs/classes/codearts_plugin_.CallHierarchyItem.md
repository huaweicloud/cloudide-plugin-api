[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CallHierarchyItem

# Class: CallHierarchyItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).CallHierarchyItem

Represents programming constructs like functions or constructors in the context
of call hierarchy.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.CallHierarchyItem.md#constructor)

### Properties

- [detail](codearts_plugin_.CallHierarchyItem.md#detail)
- [kind](codearts_plugin_.CallHierarchyItem.md#kind)
- [name](codearts_plugin_.CallHierarchyItem.md#name)
- [range](codearts_plugin_.CallHierarchyItem.md#range)
- [selectionRange](codearts_plugin_.CallHierarchyItem.md#selectionrange)
- [tags](codearts_plugin_.CallHierarchyItem.md#tags)
- [uri](codearts_plugin_.CallHierarchyItem.md#uri)

## Constructors

### constructor

• **new CallHierarchyItem**(`kind`, `name`, `detail`, `uri`, `range`, `selectionRange`)

Creates a new call hierarchy item.

#### Parameters

| Name | Type |
| :------ | :------ |
| `kind` | [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md) |
| `name` | `string` |
| `detail` | `string` |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) |
| `range` | [`Range`](codearts_plugin_.Range.md) |
| `selectionRange` | [`Range`](codearts_plugin_.Range.md) |

#### Defined in

[index.d.ts:5249](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5249)

## Properties

### detail

• `Optional` **detail**: `string`

More detail for this item, e.g. the signature of a function.

#### Defined in

[index.d.ts:5228](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5228)

___

### kind

• **kind**: [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md)

The kind of this item.

#### Defined in

[index.d.ts:5218](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5218)

___

### name

• **name**: `string`

The name of this item.

#### Defined in

[index.d.ts:5213](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5213)

___

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

The range enclosing this symbol not including leading/trailing whitespace but everything else, e.g. comments and code.

#### Defined in

[index.d.ts:5238](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5238)

___

### selectionRange

• **selectionRange**: [`Range`](codearts_plugin_.Range.md)

The range that should be selected and revealed when this symbol is being picked, e.g. the name of a function.
Must be contained by the [`range`](codearts_plugin_.CallHierarchyItem.md#range).

#### Defined in

[index.d.ts:5244](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5244)

___

### tags

• `Optional` **tags**: readonly [`Deprecated`](../enums/codearts_plugin_.SymbolTag.md#deprecated)[]

Tags for this item.

#### Defined in

[index.d.ts:5223](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5223)

___

### uri

• **uri**: [`Uri`](codearts_plugin_.Uri.md)

The resource identifier of this item.

#### Defined in

[index.d.ts:5233](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5233)
