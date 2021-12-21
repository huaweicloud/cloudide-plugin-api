**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DecorationRangeBehavior

# Enumeration: DecorationRangeBehavior

Describes the behavior of decorations when typing/editing at their edges.

## Index

### Enumeration members

* [ClosedClosed](_index_d_._plugin_.decorationrangebehavior.md#closedclosed)
* [ClosedOpen](_index_d_._plugin_.decorationrangebehavior.md#closedopen)
* [OpenClosed](_index_d_._plugin_.decorationrangebehavior.md#openclosed)
* [OpenOpen](_index_d_._plugin_.decorationrangebehavior.md#openopen)

## Enumeration members

### ClosedClosed

•  **ClosedClosed**:  = 1

*Defined in [index.d.ts:856](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L856)*

The decoration's range will not widen when edits occur at the start of end.

___

### ClosedOpen

•  **ClosedOpen**:  = 3

*Defined in [index.d.ts:864](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L864)*

The decoration's range will widen when edits occur at the end, but not at the start.

___

### OpenClosed

•  **OpenClosed**:  = 2

*Defined in [index.d.ts:860](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L860)*

The decoration's range will widen when edits occur at the start, but not at the end.

___

### OpenOpen

•  **OpenOpen**:  = 0

*Defined in [index.d.ts:852](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L852)*

The decoration's range will widen when edits occur at the start or end.
