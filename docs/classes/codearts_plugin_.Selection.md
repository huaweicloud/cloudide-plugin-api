[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Selection

# Class: Selection

["@codearts/plugin"](../modules/_codearts_plugin_.md).Selection

Represents a text selection in an editor.

## Hierarchy

- [`Range`](codearts_plugin_.Range.md)

  ↳ **`Selection`**

## Table of contents

### Constructors

- [constructor](codearts_plugin_.Selection.md#constructor)

### Properties

- [active](codearts_plugin_.Selection.md#active)
- [anchor](codearts_plugin_.Selection.md#anchor)
- [end](codearts_plugin_.Selection.md#end)
- [isEmpty](codearts_plugin_.Selection.md#isempty)
- [isReversed](codearts_plugin_.Selection.md#isreversed)
- [isSingleLine](codearts_plugin_.Selection.md#issingleline)
- [start](codearts_plugin_.Selection.md#start)

### Methods

- [contains](codearts_plugin_.Selection.md#contains)
- [intersection](codearts_plugin_.Selection.md#intersection)
- [isEqual](codearts_plugin_.Selection.md#isequal)
- [union](codearts_plugin_.Selection.md#union)
- [with](codearts_plugin_.Selection.md#with)

## Constructors

### constructor

• **new Selection**(`anchor`, `active`)

Create a selection from two positions.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `anchor` | [`Position`](codearts_plugin_.Position.md) | A position. |
| `active` | [`Position`](codearts_plugin_.Position.md) | A position. |

#### Overrides

[Range](codearts_plugin_.Range.md).[constructor](codearts_plugin_.Range.md#constructor)

#### Defined in

[index.d.ts:499](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L499)

• **new Selection**(`anchorLine`, `anchorCharacter`, `activeLine`, `activeCharacter`)

Create a selection from four coordinates.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `anchorLine` | `number` | A zero-based line value. |
| `anchorCharacter` | `number` | A zero-based character value. |
| `activeLine` | `number` | A zero-based line value. |
| `activeCharacter` | `number` | A zero-based character value. |

#### Overrides

[Range](codearts_plugin_.Range.md).[constructor](codearts_plugin_.Range.md#constructor)

#### Defined in

[index.d.ts:509](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L509)

## Properties

### active

• **active**: [`Position`](codearts_plugin_.Position.md)

The position of the cursor.
This position might be before or after [anchor](codearts_plugin_.Selection.md#anchor).

#### Defined in

[index.d.ts:491](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L491)

___

### anchor

• **anchor**: [`Position`](codearts_plugin_.Position.md)

The position at which the selection starts.
This position might be before or after [active](codearts_plugin_.Selection.md#active).

#### Defined in

[index.d.ts:485](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L485)

___

### end

• `Readonly` **end**: [`Position`](codearts_plugin_.Position.md)

The end position. It is after or equal to [start](codearts_plugin_.Range.md#start).

#### Inherited from

[Range](codearts_plugin_.Range.md).[end](codearts_plugin_.Range.md#end)

#### Defined in

[index.d.ts:388](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L388)

___

### isEmpty

• **isEmpty**: `boolean`

`true` if `start` and `end` are equal.

#### Inherited from

[Range](codearts_plugin_.Range.md).[isEmpty](codearts_plugin_.Range.md#isempty)

#### Defined in

[index.d.ts:413](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L413)

___

### isReversed

• **isReversed**: `boolean`

A selection is reversed if its [anchor](codearts_plugin_.Selection.md#anchor) is the [end](codearts_plugin_.Selection.md#end) position.

#### Defined in

[index.d.ts:514](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L514)

___

### isSingleLine

• **isSingleLine**: `boolean`

`true` if `start.line` and `end.line` are equal.

#### Inherited from

[Range](codearts_plugin_.Range.md).[isSingleLine](codearts_plugin_.Range.md#issingleline)

#### Defined in

[index.d.ts:418](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L418)

___

### start

• `Readonly` **start**: [`Position`](codearts_plugin_.Position.md)

The start position. It is before or equal to [end](codearts_plugin_.Range.md#end).

#### Inherited from

[Range](codearts_plugin_.Range.md).[start](codearts_plugin_.Range.md#start)

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

#### Inherited from

[Range](codearts_plugin_.Range.md).[contains](codearts_plugin_.Range.md#contains)

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

#### Inherited from

[Range](codearts_plugin_.Range.md).[intersection](codearts_plugin_.Range.md#intersection)

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

#### Inherited from

[Range](codearts_plugin_.Range.md).[isEqual](codearts_plugin_.Range.md#isequal)

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

#### Inherited from

[Range](codearts_plugin_.Range.md).[union](codearts_plugin_.Range.md#union)

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

#### Inherited from

[Range](codearts_plugin_.Range.md).[with](codearts_plugin_.Range.md#with)

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

#### Inherited from

[Range](codearts_plugin_.Range.md).[with](codearts_plugin_.Range.md#with)

#### Defined in

[index.d.ts:473](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L473)
