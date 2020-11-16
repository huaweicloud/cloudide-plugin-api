**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Range

# Class: Range

A range represents an ordered pair of two positions.
It is guaranteed that [start](#Range.start).isBeforeOrEqual([end](#Range.end))

Range objects are __immutable__. Use the [with](#Range.with),
[intersection](#Range.intersection), or [union](#Range.union) methods
to derive new ranges from an existing range.

## Hierarchy

* **Range**

  ↳ [Selection](_index_d_._plugin_.selection.md)

## Index

### Constructors

* [constructor](_index_d_._plugin_.range.md#constructor)

### Properties

* [end](_index_d_._plugin_.range.md#end)
* [isEmpty](_index_d_._plugin_.range.md#isempty)
* [isSingleLine](_index_d_._plugin_.range.md#issingleline)
* [start](_index_d_._plugin_.range.md#start)

### Methods

* [contains](_index_d_._plugin_.range.md#contains)
* [intersection](_index_d_._plugin_.range.md#intersection)
* [isEqual](_index_d_._plugin_.range.md#isequal)
* [union](_index_d_._plugin_.range.md#union)
* [with](_index_d_._plugin_.range.md#with)

## Constructors

### constructor

\+ **new Range**(`start`: [Position](_index_d_._plugin_.position.md), `end`: [Position](_index_d_._plugin_.position.md)): [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:388](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L388)*

Create a new range from two positions. If `start` is not
before or equal to `end`, the values will be swapped.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`start` | [Position](_index_d_._plugin_.position.md) | A position. |
`end` | [Position](_index_d_._plugin_.position.md) | A position.  |

**Returns:** [Range](_index_d_._plugin_.range.md)

\+ **new Range**(`startLine`: number, `startCharacter`: number, `endLine`: number, `endCharacter`: number): [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:397](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L397)*

Create a new range from number coordinates. It is a shorter equivalent of
using `new Range(new Position(startLine, startCharacter), new Position(endLine, endCharacter))`

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`startLine` | number | A zero-based line value. |
`startCharacter` | number | A zero-based character value. |
`endLine` | number | A zero-based line value. |
`endCharacter` | number | A zero-based character value.  |

**Returns:** [Range](_index_d_._plugin_.range.md)

## Properties

### end

• `Readonly` **end**: [Position](_index_d_._plugin_.position.md)

*Defined in [index.d.ts:388](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L388)*

The end position. It is after or equal to [start](#Range.start).

___

### isEmpty

•  **isEmpty**: boolean

*Defined in [index.d.ts:413](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L413)*

`true` if `start` and `end` are equal.

___

### isSingleLine

•  **isSingleLine**: boolean

*Defined in [index.d.ts:418](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L418)*

`true` if `start.line` and `end.line` are equal.

___

### start

• `Readonly` **start**: [Position](_index_d_._plugin_.position.md)

*Defined in [index.d.ts:383](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L383)*

The start position. It is before or equal to [end](#Range.end).

## Methods

### contains

▸ **contains**(`positionOrRange`: [Position](_index_d_._plugin_.position.md) \| [Range](_index_d_._plugin_.range.md)): boolean

*Defined in [index.d.ts:427](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L427)*

Check if a position or a range is contained in this range.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`positionOrRange` | [Position](_index_d_._plugin_.position.md) \| [Range](_index_d_._plugin_.range.md) | A position or a range. |

**Returns:** boolean

`true` if the position or range is inside or equal
to this range.

___

### intersection

▸ **intersection**(`range`: [Range](_index_d_._plugin_.range.md)): [Range](_index_d_._plugin_.range.md) \| undefined

*Defined in [index.d.ts:446](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L446)*

Intersect `range` with this range and returns a new range or `undefined`
if the ranges have no overlap.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`range` | [Range](_index_d_._plugin_.range.md) | A range. |

**Returns:** [Range](_index_d_._plugin_.range.md) \| undefined

A range of the greater start and smaller end positions. Will
return undefined when there is no overlap.

___

### isEqual

▸ **isEqual**(`other`: [Range](_index_d_._plugin_.range.md)): boolean

*Defined in [index.d.ts:436](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L436)*

Check if `other` equals this range.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`other` | [Range](_index_d_._plugin_.range.md) | A range. |

**Returns:** boolean

`true` when start and end are [equal](#Position.isEqual) to
start and end of this range.

___

### union

▸ **union**(`other`: [Range](_index_d_._plugin_.range.md)): [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:454](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L454)*

Compute the union of `other` with this range.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`other` | [Range](_index_d_._plugin_.range.md) | A range. |

**Returns:** [Range](_index_d_._plugin_.range.md)

A range of smaller start position and the greater end position.

___

### with

▸ **with**(`start?`: [Position](_index_d_._plugin_.position.md), `end?`: [Position](_index_d_._plugin_.position.md)): [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:464](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L464)*

Derived a new range from this range.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`start?` | [Position](_index_d_._plugin_.position.md) | A position that should be used as start. The default value is the [current start](#Range.start). |
`end?` | [Position](_index_d_._plugin_.position.md) | A position that should be used as end. The default value is the [current end](#Range.end). |

**Returns:** [Range](_index_d_._plugin_.range.md)

A range derived from this range with the given start and end position.
If start and end are not different `this` range will be returned.

▸ **with**(`change`: { end?: [Position](_index_d_._plugin_.position.md) ; start?: [Position](_index_d_._plugin_.position.md)  }): [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:473](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L473)*

Derived a new range from this range.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`change` | { end?: [Position](_index_d_._plugin_.position.md) ; start?: [Position](_index_d_._plugin_.position.md)  } | An object that describes a change to this range. |

**Returns:** [Range](_index_d_._plugin_.range.md)

A range that reflects the given change. Will return `this` range if the change
is not changing anything.
