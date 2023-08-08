[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SymbolInformation

# Class: SymbolInformation

["@codearts/plugin"](../modules/_codearts_plugin_.md).SymbolInformation

Represents information about programming constructs like variables, classes,
interfaces etc.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.SymbolInformation.md#constructor)

### Properties

- [containerName](codearts_plugin_.SymbolInformation.md#containername)
- [kind](codearts_plugin_.SymbolInformation.md#kind)
- [location](codearts_plugin_.SymbolInformation.md#location)
- [name](codearts_plugin_.SymbolInformation.md#name)
- [tags](codearts_plugin_.SymbolInformation.md#tags)

## Constructors

### constructor

• **new SymbolInformation**(`name`, `kind`, `containerName`, `location`)

Creates a new symbol information object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the symbol. |
| `kind` | [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md) | The kind of the symbol. |
| `containerName` | `string` | The name of the symbol containing the symbol. |
| `location` | [`Location`](codearts_plugin_.Location.md) | The location of the symbol. |

#### Defined in

[index.d.ts:3202](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3202)

• **new SymbolInformation**(`name`, `kind`, `range`, `uri?`, `containerName?`)

Creates a new symbol information object.

**`Deprecated`**

Please use the constructor taking a [Location](codearts_plugin_.Location.md) object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the symbol. |
| `kind` | [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md) | The kind of the symbol. |
| `range` | [`Range`](codearts_plugin_.Range.md) | The range of the location of the symbol. |
| `uri?` | [`Uri`](codearts_plugin_.Uri.md) | The resource of the location of symbol, defaults to the current document. |
| `containerName?` | `string` | The name of the symbol containing the symbol. |

#### Defined in

[index.d.ts:3215](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3215)

## Properties

### containerName

• **containerName**: `string`

The name of the symbol containing this symbol.

#### Defined in

[index.d.ts:3177](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3177)

___

### kind

• **kind**: [`SymbolKind`](../enums/codearts_plugin_.SymbolKind.md)

The kind of this symbol.

#### Defined in

[index.d.ts:3182](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3182)

___

### location

• **location**: [`Location`](codearts_plugin_.Location.md)

The location of this symbol.

#### Defined in

[index.d.ts:3192](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3192)

___

### name

• **name**: `string`

The name of this symbol.

#### Defined in

[index.d.ts:3172](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3172)

___

### tags

• `Optional` **tags**: readonly [`Deprecated`](../enums/codearts_plugin_.SymbolTag.md#deprecated)[]

Tags for this symbol.

#### Defined in

[index.d.ts:3187](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L3187)
