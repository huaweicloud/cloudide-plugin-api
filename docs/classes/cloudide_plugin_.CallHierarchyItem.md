[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CallHierarchyItem

# Class: CallHierarchyItem

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CallHierarchyItem

Represents programming constructs like functions or constructors in the context
of call hierarchy.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.CallHierarchyItem.md#constructor)

### Properties

- [data](cloudide_plugin_.CallHierarchyItem.md#data)
- [detail](cloudide_plugin_.CallHierarchyItem.md#detail)
- [kind](cloudide_plugin_.CallHierarchyItem.md#kind)
- [name](cloudide_plugin_.CallHierarchyItem.md#name)
- [range](cloudide_plugin_.CallHierarchyItem.md#range)
- [selectionRange](cloudide_plugin_.CallHierarchyItem.md#selectionrange)
- [tags](cloudide_plugin_.CallHierarchyItem.md#tags)
- [uri](cloudide_plugin_.CallHierarchyItem.md#uri)

## Constructors

### constructor

• **new CallHierarchyItem**(`kind`, `name`, `detail`, `uri`, `range`, `selectionRange`)

Creates a new call hierarchy item.

#### Parameters

| Name | Type |
| :------ | :------ |
| `kind` | [`SymbolKind`](../enums/cloudide_plugin_.SymbolKind.md) |
| `name` | `string` |
| `detail` | `string` |
| `uri` | [`Uri`](cloudide_plugin_.Uri.md) |
| `range` | [`Range`](cloudide_plugin_.Range.md) |
| `selectionRange` | [`Range`](cloudide_plugin_.Range.md) |

#### Defined in

[index.d.ts:11181](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11181)

## Properties

### data

• `Optional` **data**: `unknown`

A data entry field that is preserved between a call hierarchy prepare and
incoming calls or outgoing calls requests.

#### Defined in

[index.d.ts:11176](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11176)

___

### detail

• `Optional` **detail**: `string`

More detail for this item, e.g. the signature of a function.

#### Defined in

[index.d.ts:11149](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11149)

___

### kind

• **kind**: [`SymbolKind`](../enums/cloudide_plugin_.SymbolKind.md)

The kind of this item.

#### Defined in

[index.d.ts:11144](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11144)

___

### name

• **name**: `string`

The name of this item.

#### Defined in

[index.d.ts:11139](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11139)

___

### range

• **range**: [`Range`](cloudide_plugin_.Range.md)

The range enclosing this symbol not including leading/trailing whitespace but everything else, e.g. comments and code.

#### Defined in

[index.d.ts:11159](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11159)

___

### selectionRange

• **selectionRange**: [`Range`](cloudide_plugin_.Range.md)

The range that should be selected and revealed when this symbol is being picked, e.g. the name of a function.
Must be contained by the [`range`](#CallHierarchyItem.range).

#### Defined in

[index.d.ts:11165](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11165)

___

### tags

• `Optional` **tags**: readonly [`Deprecated`](../enums/cloudide_plugin_.SymbolTag.md#deprecated)[]

Tags for this item.

#### Defined in

[index.d.ts:11170](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11170)

___

### uri

• **uri**: [`Uri`](cloudide_plugin_.Uri.md)

The resource identifier of this item.

#### Defined in

[index.d.ts:11154](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11154)
