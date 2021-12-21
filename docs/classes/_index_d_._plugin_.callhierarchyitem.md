**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CallHierarchyItem

# Class: CallHierarchyItem

Represents programming constructs like functions or constructors in the context
of call hierarchy.

## Hierarchy

* **CallHierarchyItem**

## Index

### Constructors

* [constructor](_index_d_._plugin_.callhierarchyitem.md#constructor)

### Properties

* [detail](_index_d_._plugin_.callhierarchyitem.md#detail)
* [kind](_index_d_._plugin_.callhierarchyitem.md#kind)
* [name](_index_d_._plugin_.callhierarchyitem.md#name)
* [range](_index_d_._plugin_.callhierarchyitem.md#range)
* [selectionRange](_index_d_._plugin_.callhierarchyitem.md#selectionrange)
* [tags](_index_d_._plugin_.callhierarchyitem.md#tags)
* [uri](_index_d_._plugin_.callhierarchyitem.md#uri)

## Constructors

### constructor

\+ **new CallHierarchyItem**(`kind`: [SymbolKind](../enums/_index_d_._plugin_.symbolkind.md), `name`: string, `detail`: string, `uri`: [Uri](_index_d_._plugin_.uri.md), `range`: [Range](_index_d_._plugin_.range.md), `selectionRange`: [Range](_index_d_._plugin_.range.md)): [CallHierarchyItem](_index_d_._plugin_.callhierarchyitem.md)

*Defined in [index.d.ts:4572](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4572)*

Creates a new call hierarchy item.

#### Parameters:

Name | Type |
------ | ------ |
`kind` | [SymbolKind](../enums/_index_d_._plugin_.symbolkind.md) |
`name` | string |
`detail` | string |
`uri` | [Uri](_index_d_._plugin_.uri.md) |
`range` | [Range](_index_d_._plugin_.range.md) |
`selectionRange` | [Range](_index_d_._plugin_.range.md) |

**Returns:** [CallHierarchyItem](_index_d_._plugin_.callhierarchyitem.md)

## Properties

### detail

• `Optional` **detail**: string

*Defined in [index.d.ts:4556](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4556)*

More detail for this item, e.g. the signature of a function.

___

### kind

•  **kind**: [SymbolKind](../enums/_index_d_._plugin_.symbolkind.md)

*Defined in [index.d.ts:4546](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4546)*

The kind of this item.

___

### name

•  **name**: string

*Defined in [index.d.ts:4541](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4541)*

The name of this item.

___

### range

•  **range**: [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:4566](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4566)*

The range enclosing this symbol not including leading/trailing whitespace but everything else, e.g. comments and code.

___

### selectionRange

•  **selectionRange**: [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:4572](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4572)*

The range that should be selected and revealed when this symbol is being picked, e.g. the name of a function.
Must be contained by the [`range`](#CallHierarchyItem.range).

___

### tags

• `Optional` **tags**: ReadonlyArray\<[SymbolTag](../enums/_index_d_._plugin_.symboltag.md)>

*Defined in [index.d.ts:4551](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4551)*

Tags for this item.

___

### uri

•  **uri**: [Uri](_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:4561](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L4561)*

The resource identifier of this item.
