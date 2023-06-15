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

[index.d.ts:5198](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5198)

## Properties

### detail

• `Optional` **detail**: `string`

More detail for this item, e.g. the signature of a function.

#### Defined in

[index.d.ts:5177](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5177)

___

### kind

• **kind**: [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md)

The kind of this item.

#### Defined in

[index.d.ts:5167](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5167)

___

### name

• **name**: `string`

The name of this item.

#### Defined in

[index.d.ts:5162](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5162)

___

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

The range enclosing this symbol not including leading/trailing whitespace but everything else, e.g. comments and code.

#### Defined in

[index.d.ts:5187](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5187)

___

### selectionRange

• **selectionRange**: [`Range`](codearts_plugin_.Range.md)

The range that should be selected and revealed when this symbol is being picked, e.g. the name of a function.
Must be contained by the [`range`](codearts_plugin_.CallHierarchyItem.md#range).

#### Defined in

[index.d.ts:5193](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5193)

___

### tags

• `Optional` **tags**: readonly [`Deprecated`](../enums/codearts_plugin_.SymbolTag.md#deprecated)[]

Tags for this item.

#### Defined in

[index.d.ts:5172](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5172)

___

### uri

• **uri**: [`Uri`](codearts_plugin_.Uri.md)

The resource identifier of this item.

#### Defined in

[index.d.ts:5182](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L5182)
