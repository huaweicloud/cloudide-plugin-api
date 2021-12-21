**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Position

# Class: Position

Represents a line and character position, such as
the position of the cursor.

Position objects are __immutable__. Use the [with](#Position.with) or
[translate](#Position.translate) methods to derive new positions
from an existing position.

## Hierarchy

* **Position**

## Index

### Constructors

* [constructor](_index_d_._plugin_.position.md#constructor)

### Properties

* [character](_index_d_._plugin_.position.md#character)
* [line](_index_d_._plugin_.position.md#line)

### Methods

* [compareTo](_index_d_._plugin_.position.md#compareto)
* [isAfter](_index_d_._plugin_.position.md#isafter)
* [isAfterOrEqual](_index_d_._plugin_.position.md#isafterorequal)
* [isBefore](_index_d_._plugin_.position.md#isbefore)
* [isBeforeOrEqual](_index_d_._plugin_.position.md#isbeforeorequal)
* [isEqual](_index_d_._plugin_.position.md#isequal)
* [translate](_index_d_._plugin_.position.md#translate)
* [with](_index_d_._plugin_.position.md#with)

## Constructors

### constructor

\+ **new Position**(`line`: number, `character`: number): [Position](_index_d_._plugin_.position.md)

*Defined in [index.d.ts:379](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L379)*

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`line` | number | A zero-based line value. |
`character` | number | A zero-based character value.  |

**Returns:** [Position](_index_d_._plugin_.position.md)

## Properties

### character

• `Readonly` **character**: number

*Defined in [index.d.ts:379](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L379)*

The zero-based character value.

___

### line

• `Readonly` **line**: number

*Defined in [index.d.ts:374](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L374)*

The zero-based line value.

## Methods

### compareTo

▸ **compareTo**(`other`: [Position](_index_d_._plugin_.position.md)): number

*Defined in [index.d.ts:440](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L440)*

Compare this to `other`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`other` | [Position](_index_d_._plugin_.position.md) | A position. |

**Returns:** number

A number smaller than zero if this position is before the given position,
a number greater than zero if this position is after the given position, or zero when
this and the given position are equal.

___

### isAfter

▸ **isAfter**(`other`: [Position](_index_d_._plugin_.position.md)): boolean

*Defined in [index.d.ts:412](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L412)*

Check if this position is after `other`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`other` | [Position](_index_d_._plugin_.position.md) | A position. |

**Returns:** boolean

`true` if position is on a greater line
or on the same line on a greater character.

___

### isAfterOrEqual

▸ **isAfterOrEqual**(`other`: [Position](_index_d_._plugin_.position.md)): boolean

*Defined in [index.d.ts:421](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L421)*

Check if this position is after or equal to `other`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`other` | [Position](_index_d_._plugin_.position.md) | A position. |

**Returns:** boolean

`true` if position is on a greater line
or on the same line on a greater or equal character.

___

### isBefore

▸ **isBefore**(`other`: [Position](_index_d_._plugin_.position.md)): boolean

*Defined in [index.d.ts:394](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L394)*

Check if this position is before `other`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`other` | [Position](_index_d_._plugin_.position.md) | A position. |

**Returns:** boolean

`true` if position is on a smaller line
or on the same line on a smaller character.

___

### isBeforeOrEqual

▸ **isBeforeOrEqual**(`other`: [Position](_index_d_._plugin_.position.md)): boolean

*Defined in [index.d.ts:403](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L403)*

Check if this position is before or equal to `other`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`other` | [Position](_index_d_._plugin_.position.md) | A position. |

**Returns:** boolean

`true` if position is on a smaller line
or on the same line on a smaller or equal character.

___

### isEqual

▸ **isEqual**(`other`: [Position](_index_d_._plugin_.position.md)): boolean

*Defined in [index.d.ts:430](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L430)*

Check if this position is equal to `other`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`other` | [Position](_index_d_._plugin_.position.md) | A position. |

**Returns:** boolean

`true` if the line and character of the given position are equal to
the line and character of this position.

___

### translate

▸ **translate**(`lineDelta?`: number, `characterDelta?`: number): [Position](_index_d_._plugin_.position.md)

*Defined in [index.d.ts:450](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L450)*

Create a new position relative to this position.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`lineDelta?` | number | Delta value for the line value, default is `0`. |
`characterDelta?` | number | Delta value for the character value, default is `0`. |

**Returns:** [Position](_index_d_._plugin_.position.md)

A position which line and character is the sum of the current line and
character and the corresponding deltas.

▸ **translate**(`change`: { characterDelta?: number ; lineDelta?: number  }): [Position](_index_d_._plugin_.position.md)

*Defined in [index.d.ts:459](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L459)*

Derived a new position relative to this position.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`change` | { characterDelta?: number ; lineDelta?: number  } | An object that describes a delta to this position. |

**Returns:** [Position](_index_d_._plugin_.position.md)

A position that reflects the given delta. Will return `this` position if the change
is not changing anything.

___

### with

▸ **with**(`line?`: number, `character?`: number): [Position](_index_d_._plugin_.position.md)

*Defined in [index.d.ts:468](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L468)*

Create a new position derived from this position.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`line?` | number | Value that should be used as line value, default is the [existing value](#Position.line) |
`character?` | number | Value that should be used as character value, default is the [existing value](#Position.character) |

**Returns:** [Position](_index_d_._plugin_.position.md)

A position where line and character are replaced by the given values.

▸ **with**(`change`: { character?: number ; line?: number  }): [Position](_index_d_._plugin_.position.md)

*Defined in [index.d.ts:477](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L477)*

Derived a new position from this position.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`change` | { character?: number ; line?: number  } | An object that describes a change to this position. |

**Returns:** [Position](_index_d_._plugin_.position.md)

A position that reflects the given change. Will return `this` position if the change
is not changing anything.
