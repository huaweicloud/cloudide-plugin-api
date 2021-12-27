**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Selection

# Class: Selection

Represents a text selection in an editor.

## Hierarchy

* [Range](_index_d_._plugin_.range.md)

  ↳ **Selection**

## Index

### Constructors

* [constructor](_index_d_._plugin_.selection.md#constructor)

### Properties

* [active](_index_d_._plugin_.selection.md#active)
* [anchor](_index_d_._plugin_.selection.md#anchor)
* [end](_index_d_._plugin_.selection.md#end)
* [isEmpty](_index_d_._plugin_.selection.md#isempty)
* [isReversed](_index_d_._plugin_.selection.md#isreversed)
* [isSingleLine](_index_d_._plugin_.selection.md#issingleline)
* [start](_index_d_._plugin_.selection.md#start)

### Methods

* [contains](_index_d_._plugin_.selection.md#contains)
* [intersection](_index_d_._plugin_.selection.md#intersection)
* [isEqual](_index_d_._plugin_.selection.md#isequal)
* [union](_index_d_._plugin_.selection.md#union)
* [with](_index_d_._plugin_.selection.md#with)

## Constructors

### constructor

\+ **new Selection**(`anchor`: [Position](_index_d_._plugin_.position.md), `active`: [Position](_index_d_._plugin_.position.md)): [Selection](_index_d_._plugin_.selection.md)

*Overrides [Range](_index_d_._plugin_.range.md).[constructor](_index_d_._plugin_.range.md#constructor)*

*Defined in [index.d.ts:604](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L604)*

Create a selection from two positions.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`anchor` | [Position](_index_d_._plugin_.position.md) | A position. |
`active` | [Position](_index_d_._plugin_.position.md) | A position.  |

**Returns:** [Selection](_index_d_._plugin_.selection.md)

\+ **new Selection**(`anchorLine`: number, `anchorCharacter`: number, `activeLine`: number, `activeCharacter`: number): [Selection](_index_d_._plugin_.selection.md)

*Overrides [Range](_index_d_._plugin_.range.md).[constructor](_index_d_._plugin_.range.md#constructor)*

*Defined in [index.d.ts:612](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L612)*

Create a selection from four coordinates.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`anchorLine` | number | A zero-based line value. |
`anchorCharacter` | number | A zero-based character value. |
`activeLine` | number | A zero-based line value. |
`activeCharacter` | number | A zero-based character value.  |

**Returns:** [Selection](_index_d_._plugin_.selection.md)

## Properties

### active

•  **active**: [Position](_index_d_._plugin_.position.md)

*Defined in [index.d.ts:604](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L604)*

The position of the cursor.
This position might be before or after [anchor](#Selection.anchor).

___

### anchor

•  **anchor**: [Position](_index_d_._plugin_.position.md)

*Defined in [index.d.ts:598](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L598)*

The position at which the selection starts.
This position might be before or after [active](#Selection.active).

___

### end

• `Readonly` **end**: [Position](_index_d_._plugin_.position.md)

*Inherited from [Range](_index_d_._plugin_.range.md).[end](_index_d_._plugin_.range.md#end)*

*Defined in [index.d.ts:501](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L501)*

The end position. It is after or equal to [start](#Range.start).

___

### isEmpty

•  **isEmpty**: boolean

*Inherited from [Range](_index_d_._plugin_.range.md).[isEmpty](_index_d_._plugin_.range.md#isempty)*

*Defined in [index.d.ts:526](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L526)*

`true` if `start` and `end` are equal.

___

### isReversed

•  **isReversed**: boolean

*Defined in [index.d.ts:627](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L627)*

A selection is reversed if [active](#Selection.active).isBefore([anchor](#Selection.anchor)).

___

### isSingleLine

•  **isSingleLine**: boolean

*Inherited from [Range](_index_d_._plugin_.range.md).[isSingleLine](_index_d_._plugin_.range.md#issingleline)*

*Defined in [index.d.ts:531](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L531)*

`true` if `start.line` and `end.line` are equal.

___

### start

• `Readonly` **start**: [Position](_index_d_._plugin_.position.md)

*Inherited from [Range](_index_d_._plugin_.range.md).[start](_index_d_._plugin_.range.md#start)*

*Defined in [index.d.ts:496](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L496)*

The start position. It is before or equal to [end](#Range.end).

## Methods

### contains

▸ **contains**(`positionOrRange`: [Position](_index_d_._plugin_.position.md) \| [Range](_index_d_._plugin_.range.md)): boolean

*Inherited from [Range](_index_d_._plugin_.range.md).[contains](_index_d_._plugin_.range.md#contains)*

*Defined in [index.d.ts:540](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L540)*

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

*Inherited from [Range](_index_d_._plugin_.range.md).[intersection](_index_d_._plugin_.range.md#intersection)*

*Defined in [index.d.ts:559](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L559)*

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

*Inherited from [Range](_index_d_._plugin_.range.md).[isEqual](_index_d_._plugin_.range.md#isequal)*

*Defined in [index.d.ts:549](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L549)*

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

*Inherited from [Range](_index_d_._plugin_.range.md).[union](_index_d_._plugin_.range.md#union)*

*Defined in [index.d.ts:567](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L567)*

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

*Inherited from [Range](_index_d_._plugin_.range.md).[with](_index_d_._plugin_.range.md#with)*

*Defined in [index.d.ts:577](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L577)*

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

*Inherited from [Range](_index_d_._plugin_.range.md).[with](_index_d_._plugin_.range.md#with)*

*Defined in [index.d.ts:586](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L586)*

Derived a new range from this range.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`change` | { end?: [Position](_index_d_._plugin_.position.md) ; start?: [Position](_index_d_._plugin_.position.md)  } | An object that describes a change to this range. |

**Returns:** [Range](_index_d_._plugin_.range.md)

A range that reflects the given change. Will return `this` range if the change
is not changing anything.
