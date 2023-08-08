[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / LocationLink

# Interface: LocationLink

["@codearts/plugin"](../modules/_codearts_plugin_.md).LocationLink

Represents the connection of two locations. Provides additional metadata over normal [locations](../classes/codearts_plugin_.Location.md),
including an origin range.

## Table of contents

### Properties

- [originSelectionRange](codearts_plugin_.LocationLink.md#originselectionrange)
- [targetRange](codearts_plugin_.LocationLink.md#targetrange)
- [targetSelectionRange](codearts_plugin_.LocationLink.md#targetselectionrange)
- [targetUri](codearts_plugin_.LocationLink.md#targeturi)

## Properties

### originSelectionRange

• `Optional` **originSelectionRange**: [`Range`](../classes/codearts_plugin_.Range.md)

Span of the origin of this link.

Used as the underlined span for mouse definition hover. Defaults to the word range at
the definition position.

#### Defined in

[index.d.ts:5878](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5878)

___

### targetRange

• **targetRange**: [`Range`](../classes/codearts_plugin_.Range.md)

The full target range of this link.

#### Defined in

[index.d.ts:5888](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5888)

___

### targetSelectionRange

• `Optional` **targetSelectionRange**: [`Range`](../classes/codearts_plugin_.Range.md)

The span of this link.

#### Defined in

[index.d.ts:5893](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5893)

___

### targetUri

• **targetUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The target resource identifier of this link.

#### Defined in

[index.d.ts:5883](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5883)
