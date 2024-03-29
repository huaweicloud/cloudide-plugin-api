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

[index.d.ts:5907](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5907)

___

### targetRange

• **targetRange**: [`Range`](../classes/codearts_plugin_.Range.md)

The full target range of this link.

#### Defined in

[index.d.ts:5917](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5917)

___

### targetSelectionRange

• `Optional` **targetSelectionRange**: [`Range`](../classes/codearts_plugin_.Range.md)

The span of this link.

#### Defined in

[index.d.ts:5922](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5922)

___

### targetUri

• **targetUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The target resource identifier of this link.

#### Defined in

[index.d.ts:5912](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L5912)
