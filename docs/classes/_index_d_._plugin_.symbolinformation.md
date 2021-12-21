**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SymbolInformation

# Class: SymbolInformation

Represents information about programming constructs like variables, classes,
interfaces etc.

## Hierarchy

* **SymbolInformation**

## Index

### Constructors

* [constructor](_index_d_._plugin_.symbolinformation.md#constructor)

### Properties

* [containerName](_index_d_._plugin_.symbolinformation.md#containername)
* [kind](_index_d_._plugin_.symbolinformation.md#kind)
* [location](_index_d_._plugin_.symbolinformation.md#location)
* [name](_index_d_._plugin_.symbolinformation.md#name)
* [tags](_index_d_._plugin_.symbolinformation.md#tags)

## Constructors

### constructor

\+ **new SymbolInformation**(`name`: string, `kind`: [SymbolKind](../enums/_index_d_._plugin_.symbolkind.md), `containerName`: string, `location`: [Location](_index_d_._plugin_.location.md)): [SymbolInformation](_index_d_._plugin_.symbolinformation.md)

*Defined in [index.d.ts:2923](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2923)*

Creates a new symbol information object.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`name` | string | The name of the symbol. |
`kind` | [SymbolKind](../enums/_index_d_._plugin_.symbolkind.md) | The kind of the symbol. |
`containerName` | string | The name of the symbol containing the symbol. |
`location` | [Location](_index_d_._plugin_.location.md) | The location of the symbol.  |

**Returns:** [SymbolInformation](_index_d_._plugin_.symbolinformation.md)

\+ **new SymbolInformation**(`name`: string, `kind`: [SymbolKind](../enums/_index_d_._plugin_.symbolkind.md), `range`: [Range](_index_d_._plugin_.range.md), `uri?`: [Uri](_index_d_._plugin_.uri.md), `containerName?`: string): [SymbolInformation](_index_d_._plugin_.symbolinformation.md)

*Defined in [index.d.ts:2933](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2933)*

Creates a new symbol information object.

**`deprecated`** Please use the constructor taking a [location](#Location) object.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`name` | string | The name of the symbol. |
`kind` | [SymbolKind](../enums/_index_d_._plugin_.symbolkind.md) | The kind of the symbol. |
`range` | [Range](_index_d_._plugin_.range.md) | The range of the location of the symbol. |
`uri?` | [Uri](_index_d_._plugin_.uri.md) | The resource of the location of symbol, defaults to the current document. |
`containerName?` | string | The name of the symbol containing the symbol. |

**Returns:** [SymbolInformation](_index_d_._plugin_.symbolinformation.md)

## Properties

### containerName

•  **containerName**: string

*Defined in [index.d.ts:2908](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2908)*

The name of the symbol containing this symbol.

___

### kind

•  **kind**: [SymbolKind](../enums/_index_d_._plugin_.symbolkind.md)

*Defined in [index.d.ts:2913](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2913)*

The kind of this symbol.

___

### location

•  **location**: [Location](_index_d_._plugin_.location.md)

*Defined in [index.d.ts:2923](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2923)*

The location of this symbol.

___

### name

•  **name**: string

*Defined in [index.d.ts:2903](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2903)*

The name of this symbol.

___

### tags

• `Optional` **tags**: ReadonlyArray\<[SymbolTag](../enums/_index_d_._plugin_.symboltag.md)>

*Defined in [index.d.ts:2918](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2918)*

Tags for this symbol.
