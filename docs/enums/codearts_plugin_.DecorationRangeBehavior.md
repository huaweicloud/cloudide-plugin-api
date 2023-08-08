[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DecorationRangeBehavior

# Enumeration: DecorationRangeBehavior

["@codearts/plugin"](../modules/_codearts_plugin_.md).DecorationRangeBehavior

Describes the behavior of decorations when typing/editing at their edges.

## Table of contents

### Enumeration Members

- [ClosedClosed](codearts_plugin_.DecorationRangeBehavior.md#closedclosed)
- [ClosedOpen](codearts_plugin_.DecorationRangeBehavior.md#closedopen)
- [OpenClosed](codearts_plugin_.DecorationRangeBehavior.md#openclosed)
- [OpenOpen](codearts_plugin_.DecorationRangeBehavior.md#openopen)

## Enumeration Members

### ClosedClosed

• **ClosedClosed** = ``1``

The decoration's range will not widen when edits occur at the start of end.

#### Defined in

[index.d.ts:746](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L746)

___

### ClosedOpen

• **ClosedOpen** = ``3``

The decoration's range will widen when edits occur at the end, but not at the start.

#### Defined in

[index.d.ts:754](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L754)

___

### OpenClosed

• **OpenClosed** = ``2``

The decoration's range will widen when edits occur at the start, but not at the end.

#### Defined in

[index.d.ts:750](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L750)

___

### OpenOpen

• **OpenOpen** = ``0``

The decoration's range will widen when edits occur at the start or end.

#### Defined in

[index.d.ts:742](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L742)
