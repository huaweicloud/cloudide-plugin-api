[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SymbolInformation

# Class: SymbolInformation

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SymbolInformation

Represents information about programming constructs like variables, classes,
interfaces etc.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.SymbolInformation.md#constructor)

### Properties

- [containerName](cloudide_plugin_.SymbolInformation.md#containername)
- [kind](cloudide_plugin_.SymbolInformation.md#kind)
- [location](cloudide_plugin_.SymbolInformation.md#location)
- [name](cloudide_plugin_.SymbolInformation.md#name)
- [tags](cloudide_plugin_.SymbolInformation.md#tags)

## Constructors

### constructor

• **new SymbolInformation**(`name`, `kind`, `containerName`, `location`)

Creates a new symbol information object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the symbol. |
| `kind` | [`SymbolKind`](../enums/cloudide_plugin_.SymbolKind.md) | The kind of the symbol. |
| `containerName` | `string` | The name of the symbol containing the symbol. |
| `location` | [`Location`](cloudide_plugin_.Location.md) | The location of the symbol. |

#### Defined in

[index.d.ts:7020](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7020)

• **new SymbolInformation**(`name`, `kind`, `range`, `uri?`, `containerName?`)

~~Creates a new symbol information object.~~

**`Deprecated`**

Please use the constructor taking a [location](#Location) object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the symbol. |
| `kind` | [`SymbolKind`](../enums/cloudide_plugin_.SymbolKind.md) | The kind of the symbol. |
| `range` | [`Range`](cloudide_plugin_.Range.md) | The range of the location of the symbol. |
| `uri?` | [`Uri`](cloudide_plugin_.Uri.md) | The resource of the location of symbol, defaults to the current document. |
| `containerName?` | `string` | The name of the symbol containing the symbol. |

#### Defined in

[index.d.ts:7033](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7033)

## Properties

### containerName

• **containerName**: `string`

The name of the symbol containing this symbol.

#### Defined in

[index.d.ts:6998](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6998)

___

### kind

• **kind**: [`SymbolKind`](../enums/cloudide_plugin_.SymbolKind.md)

The kind of this symbol.

#### Defined in

[index.d.ts:7003](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7003)

___

### location

• **location**: [`Location`](cloudide_plugin_.Location.md)

The location of this symbol.

#### Defined in

[index.d.ts:7010](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7010)

___

### name

• **name**: `string`

The name of this symbol.

#### Defined in

[index.d.ts:6993](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6993)

___

### tags

• `Optional` **tags**: readonly [`Deprecated`](../enums/cloudide_plugin_.SymbolTag.md#deprecated)[]

#### Defined in

[index.d.ts:7005](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7005)
