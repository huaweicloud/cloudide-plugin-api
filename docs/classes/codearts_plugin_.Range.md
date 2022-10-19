[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Range

# Class: Range

["@codearts/plugin"](../modules/_codearts_plugin_.md).Range

A range represents an ordered pair of two positions.
It is guaranteed that [start](codearts_plugin_.Range.md#start).isBeforeOrEqual([end](codearts_plugin_.Range.md#end))

Range objects are __immutable__. Use the [with](codearts_plugin_.Range.md#with),
[intersection](codearts_plugin_.Range.md#intersection), or [union](codearts_plugin_.Range.md#union) methods
to derive new ranges from an existing range.

## Hierarchy

- **`Range`**

  ↳ [`Selection`](codearts_plugin_.Selection.md)

## Table of contents

### Constructors

- [constructor](codearts_plugin_.Range.md#constructor)

### Properties

- [end](codearts_plugin_.Range.md#end)
- [isEmpty](codearts_plugin_.Range.md#isempty)
- [isSingleLine](codearts_plugin_.Range.md#issingleline)
- [start](codearts_plugin_.Range.md#start)

### Methods

- [contains](codearts_plugin_.Range.md#contains)
- [intersection](codearts_plugin_.Range.md#intersection)
- [isEqual](codearts_plugin_.Range.md#isequal)
- [union](codearts_plugin_.Range.md#union)
- [with](codearts_plugin_.Range.md#with)

## Constructors

### constructor

• **new Range**(`start`, `end`)

Create a new range from two positions. If `start` is not
before or equal to `end`, the values will be swapped.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | [`Position`](codearts_plugin_.Position.md) | A position. |
| `end` | [`Position`](codearts_plugin_.Position.md) | A position. |

#### Defined in

[index.d.ts:397](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L397)

• **new Range**(`startLine`, `startCharacter`, `endLine`, `endCharacter`)

Create a new range from number coordinates. It is a shorter equivalent of
using `new Range(new Position(startLine, startCharacter), new Position(endLine, endCharacter))`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startLine` | `number` | A zero-based line value. |
| `startCharacter` | `number` | A zero-based character value. |
| `endLine` | `number` | A zero-based line value. |
| `endCharacter` | `number` | A zero-based character value. |

#### Defined in

[index.d.ts:408](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L408)

## Properties

### end

• `Readonly` **end**: [`Position`](codearts_plugin_.Position.md)

The end position. It is after or equal to [start](codearts_plugin_.Range.md#start).

#### Defined in

[index.d.ts:388](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L388)

___

### isEmpty

• **isEmpty**: `boolean`

`true` if `start` and `end` are equal.

#### Defined in

[index.d.ts:413](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L413)

___

### isSingleLine

• **isSingleLine**: `boolean`

`true` if `start.line` and `end.line` are equal.

#### Defined in

[index.d.ts:418](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L418)

___

### start

• `Readonly` **start**: [`Position`](codearts_plugin_.Position.md)

The start position. It is before or equal to [end](codearts_plugin_.Range.md#end).

#### Defined in

[index.d.ts:383](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L383)

## Methods

### contains

▸ **contains**(`positionOrRange`): `boolean`

Check if a position or a range is contained in this range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `positionOrRange` | [`Range`](codearts_plugin_.Range.md) \| [`Position`](codearts_plugin_.Position.md) | A position or a range. |

#### Returns

`boolean`

`true` if the position or range is inside or equal
to this range.

#### Defined in

[index.d.ts:427](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L427)

___

### intersection

▸ **intersection**(`range`): `undefined` \| [`Range`](codearts_plugin_.Range.md)

Intersect `range` with this range and returns a new range or `undefined`
if the ranges have no overlap.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) | A range. |

#### Returns

`undefined` \| [`Range`](codearts_plugin_.Range.md)

A range of the greater start and smaller end positions. Will
return undefined when there is no overlap.

#### Defined in

[index.d.ts:446](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L446)

___

### isEqual

▸ **isEqual**(`other`): `boolean`

Check if `other` equals this range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Range`](codearts_plugin_.Range.md) | A range. |

#### Returns

`boolean`

`true` when start and end are [equal](codearts_plugin_.Position.md#isequal) to
start and end of this range.

#### Defined in

[index.d.ts:436](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L436)

___

### union

▸ **union**(`other`): [`Range`](codearts_plugin_.Range.md)

Compute the union of `other` with this range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Range`](codearts_plugin_.Range.md) | A range. |

#### Returns

[`Range`](codearts_plugin_.Range.md)

A range of smaller start position and the greater end position.

#### Defined in

[index.d.ts:454](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L454)

___

### with

▸ **with**(`start?`, `end?`): [`Range`](codearts_plugin_.Range.md)

Derived a new range from this range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start?` | [`Position`](codearts_plugin_.Position.md) | A position that should be used as start. The default value is the [current start](codearts_plugin_.Range.md#start). |
| `end?` | [`Position`](codearts_plugin_.Position.md) | A position that should be used as end. The default value is the [current end](codearts_plugin_.Range.md#end). |

#### Returns

[`Range`](codearts_plugin_.Range.md)

A range derived from this range with the given start and end position.
If start and end are not different `this` range will be returned.

#### Defined in

[index.d.ts:464](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L464)

▸ **with**(`change`): [`Range`](codearts_plugin_.Range.md)

Derived a new range from this range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `change` | `Object` | An object that describes a change to this range. |
| `change.end?` | [`Position`](codearts_plugin_.Position.md) | - |
| `change.start?` | [`Position`](codearts_plugin_.Position.md) | - |

#### Returns

[`Range`](codearts_plugin_.Range.md)

A range that reflects the given change. Will return `this` range if the change
is not changing anything.

#### Defined in

[index.d.ts:473](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L473)
