**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DocumentSymbol

# Class: DocumentSymbol

Represents programming constructs like variables, classes, interfaces etc. that appear in a document. Document
symbols can be hierarchical and they have two ranges: one that encloses its definition and one that points to
its most interesting range, e.g. the range of an identifier.

## Hierarchy

* **DocumentSymbol**

## Index

### Constructors

* [constructor](_index_d_._plugin_.documentsymbol.md#constructor)

### Properties

* [children](_index_d_._plugin_.documentsymbol.md#children)
* [detail](_index_d_._plugin_.documentsymbol.md#detail)
* [kind](_index_d_._plugin_.documentsymbol.md#kind)
* [name](_index_d_._plugin_.documentsymbol.md#name)
* [range](_index_d_._plugin_.documentsymbol.md#range)
* [selectionRange](_index_d_._plugin_.documentsymbol.md#selectionrange)
* [tags](_index_d_._plugin_.documentsymbol.md#tags)

## Constructors

### constructor

\+ **new DocumentSymbol**(`name`: string, `detail`: string, `kind`: [SymbolKind](../enums/_index_d_._plugin_.symbolkind.md), `range`: [Range](_index_d_._plugin_.range.md), `selectionRange`: [Range](_index_d_._plugin_.range.md)): [DocumentSymbol](_index_d_._plugin_.documentsymbol.md)

*Defined in [index.d.ts:2764](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2764)*

Creates a new document symbol.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`name` | string | The name of the symbol. |
`detail` | string | Details for the symbol. |
`kind` | [SymbolKind](../enums/_index_d_._plugin_.symbolkind.md) | The kind of the symbol. |
`range` | [Range](_index_d_._plugin_.range.md) | The full range of the symbol. |
`selectionRange` | [Range](_index_d_._plugin_.range.md) | The range that should be reveal.  |

**Returns:** [DocumentSymbol](_index_d_._plugin_.documentsymbol.md)

## Properties

### children

•  **children**: [DocumentSymbol](_index_d_._plugin_.documentsymbol.md)[]

*Defined in [index.d.ts:2764](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2764)*

Children of this symbol, e.g. properties of a class.

___

### detail

•  **detail**: string

*Defined in [index.d.ts:2738](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2738)*

More detail for this symbol, e.g. the signature of a function.

___

### kind

•  **kind**: [SymbolKind](../enums/_index_d_._plugin_.symbolkind.md)

*Defined in [index.d.ts:2743](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2743)*

The kind of this symbol.

___

### name

•  **name**: string

*Defined in [index.d.ts:2733](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2733)*

The name of this symbol.

___

### range

•  **range**: [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:2753](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2753)*

The range enclosing this symbol not including leading/trailing whitespace but everything else, e.g. comments and code.

___

### selectionRange

•  **selectionRange**: [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:2759](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2759)*

The range that should be selected and reveal when this symbol is being picked, e.g. the name of a function.
Must be contained by the [`range`](#DocumentSymbol.range).

___

### tags

• `Optional` **tags**: ReadonlyArray\<[SymbolTag](../enums/_index_d_._plugin_.symboltag.md)>

*Defined in [index.d.ts:2748](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2748)*

Tags for this symbol.
