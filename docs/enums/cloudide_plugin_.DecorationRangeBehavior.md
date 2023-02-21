[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DecorationRangeBehavior

# Enumeration: DecorationRangeBehavior

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DecorationRangeBehavior

Describes the behavior of decorations when typing/editing at their edges.

## Table of contents

### Enumeration Members

- [ClosedClosed](cloudide_plugin_.DecorationRangeBehavior.md#closedclosed)
- [ClosedOpen](cloudide_plugin_.DecorationRangeBehavior.md#closedopen)
- [OpenClosed](cloudide_plugin_.DecorationRangeBehavior.md#openclosed)
- [OpenOpen](cloudide_plugin_.DecorationRangeBehavior.md#openopen)

## Enumeration Members

### ClosedClosed

• **ClosedClosed** = ``1``

The decoration's range will not widen when edits occur at the start of end.

#### Defined in

[index.d.ts:1083](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1083)

___

### ClosedOpen

• **ClosedOpen** = ``3``

The decoration's range will widen when edits occur at the end, but not at the start.

#### Defined in

[index.d.ts:1091](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1091)

___

### OpenClosed

• **OpenClosed** = ``2``

The decoration's range will widen when edits occur at the start, but not at the end.

#### Defined in

[index.d.ts:1087](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1087)

___

### OpenOpen

• **OpenOpen** = ``0``

The decoration's range will widen when edits occur at the start or end.

#### Defined in

[index.d.ts:1079](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1079)
