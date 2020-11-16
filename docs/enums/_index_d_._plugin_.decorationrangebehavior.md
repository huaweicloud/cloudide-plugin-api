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

*Defined in [index.d.ts:746](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L746)*

The decoration's range will not widen when edits occur at the start of end.

___

### ClosedOpen

•  **ClosedOpen**:  = 3

*Defined in [index.d.ts:754](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L754)*

The decoration's range will widen when edits occur at the end, but not at the start.

___

### OpenClosed

•  **OpenClosed**:  = 2

*Defined in [index.d.ts:750](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L750)*

The decoration's range will widen when edits occur at the start, but not at the end.

___

### OpenOpen

•  **OpenOpen**:  = 0

*Defined in [index.d.ts:742](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L742)*

The decoration's range will widen when edits occur at the start or end.
