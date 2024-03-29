[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TypeHierarchyItem

# Class: TypeHierarchyItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).TypeHierarchyItem

Represents an item of a type hierarchy, like a class or an interface.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.TypeHierarchyItem.md#constructor)

### Properties

- [detail](codearts_plugin_.TypeHierarchyItem.md#detail)
- [kind](codearts_plugin_.TypeHierarchyItem.md#kind)
- [name](codearts_plugin_.TypeHierarchyItem.md#name)
- [range](codearts_plugin_.TypeHierarchyItem.md#range)
- [selectionRange](codearts_plugin_.TypeHierarchyItem.md#selectionrange)
- [tags](codearts_plugin_.TypeHierarchyItem.md#tags)
- [uri](codearts_plugin_.TypeHierarchyItem.md#uri)

## Constructors

### constructor

• **new TypeHierarchyItem**(`kind`, `name`, `detail`, `uri`, `range`, `selectionRange`)

Creates a new type hierarchy item.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md) | The kind of the item. |
| `name` | `string` | The name of the item. |
| `detail` | `string` | The details of the item. |
| `uri` | [`Uri`](codearts_plugin_.Uri.md) | The Uri of the item. |
| `range` | [`Range`](codearts_plugin_.Range.md) | The whole range of the item. |
| `selectionRange` | [`Range`](codearts_plugin_.Range.md) | The selection range of the item. |

#### Defined in

[index.d.ts:5399](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5399)

## Properties

### detail

• `Optional` **detail**: `string`

More detail for this item, e.g. the signature of a function.

#### Defined in

[index.d.ts:5370](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5370)

___

### kind

• **kind**: [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md)

The kind of this item.

#### Defined in

[index.d.ts:5360](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5360)

___

### name

• **name**: `string`

The name of this item.

#### Defined in

[index.d.ts:5355](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5355)

___

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

The range enclosing this symbol not including leading/trailing whitespace
but everything else, e.g. comments and code.

#### Defined in

[index.d.ts:5381](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5381)

___

### selectionRange

• **selectionRange**: [`Range`](codearts_plugin_.Range.md)

The range that should be selected and revealed when this symbol is being
picked, e.g. the name of a class. Must be contained by the [range](codearts_plugin_.TypeHierarchyItem.md#range)-property.

#### Defined in

[index.d.ts:5387](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5387)

___

### tags

• `Optional` **tags**: readonly [`Deprecated`](../enums/codearts_plugin_.SymbolTag.md#deprecated)[]

Tags for this item.

#### Defined in

[index.d.ts:5365](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5365)

___

### uri

• **uri**: [`Uri`](codearts_plugin_.Uri.md)

The resource identifier of this item.

#### Defined in

[index.d.ts:5375](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5375)
