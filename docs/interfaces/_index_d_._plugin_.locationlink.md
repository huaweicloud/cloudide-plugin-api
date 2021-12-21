**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / LocationLink

# Interface: LocationLink

Represents the connection of two locations. Provides additional metadata over normal [locations](#Location),
including an origin range.

## Hierarchy

* **LocationLink**

## Index

### Properties

* [originSelectionRange](_index_d_._plugin_.locationlink.md#originselectionrange)
* [targetRange](_index_d_._plugin_.locationlink.md#targetrange)
* [targetSelectionRange](_index_d_._plugin_.locationlink.md#targetselectionrange)
* [targetUri](_index_d_._plugin_.locationlink.md#targeturi)

## Properties

### originSelectionRange

• `Optional` **originSelectionRange**: [Range](../classes/_index_d_._plugin_.range.md)

*Defined in [index.d.ts:5114](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5114)*

Span of the origin of this link.

Used as the underlined span for mouse definition hover. Defaults to the word range at
the definition position.

___

### targetRange

•  **targetRange**: [Range](../classes/_index_d_._plugin_.range.md)

*Defined in [index.d.ts:5124](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5124)*

The full target range of this link.

___

### targetSelectionRange

• `Optional` **targetSelectionRange**: [Range](../classes/_index_d_._plugin_.range.md)

*Defined in [index.d.ts:5129](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5129)*

The span of this link.

___

### targetUri

•  **targetUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:5119](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5119)*

The target resource identifier of this link.
