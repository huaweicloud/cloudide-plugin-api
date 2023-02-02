[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Position

# Class: Position

["@codearts/plugin"](../modules/_codearts_plugin_.md).Position

Represents a line and character position, such as
the position of the cursor.

Position objects are __immutable__. Use the [with](codearts_plugin_.Position.md#with) or
[translate](codearts_plugin_.Position.md#translate) methods to derive new positions
from an existing position.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.Position.md#constructor)

### Properties

- [character](codearts_plugin_.Position.md#character)
- [line](codearts_plugin_.Position.md#line)

### Methods

- [compareTo](codearts_plugin_.Position.md#compareto)
- [isAfter](codearts_plugin_.Position.md#isafter)
- [isAfterOrEqual](codearts_plugin_.Position.md#isafterorequal)
- [isBefore](codearts_plugin_.Position.md#isbefore)
- [isBeforeOrEqual](codearts_plugin_.Position.md#isbeforeorequal)
- [isEqual](codearts_plugin_.Position.md#isequal)
- [translate](codearts_plugin_.Position.md#translate)
- [with](codearts_plugin_.Position.md#with)

## Constructors

### constructor

• **new Position**(`line`, `character`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `line` | `number` | A zero-based line value. |
| `character` | `number` | A zero-based character value. |

#### Defined in

[index.d.ts:275](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L275)

## Properties

### character

• `Readonly` **character**: `number`

The zero-based character value.

#### Defined in

[index.d.ts:269](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L269)

___

### line

• `Readonly` **line**: `number`

The zero-based line value.

#### Defined in

[index.d.ts:264](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L264)

## Methods

### compareTo

▸ **compareTo**(`other`): `number`

Compare this to `other`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](codearts_plugin_.Position.md) | A position. |

#### Returns

`number`

A number smaller than zero if this position is before the given position,
a number greater than zero if this position is after the given position, or zero when
this and the given position are equal.

#### Defined in

[index.d.ts:330](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L330)

___

### isAfter

▸ **isAfter**(`other`): `boolean`

Check if this position is after `other`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](codearts_plugin_.Position.md) | A position. |

#### Returns

`boolean`

`true` if position is on a greater line
or on the same line on a greater character.

#### Defined in

[index.d.ts:302](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L302)

___

### isAfterOrEqual

▸ **isAfterOrEqual**(`other`): `boolean`

Check if this position is after or equal to `other`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](codearts_plugin_.Position.md) | A position. |

#### Returns

`boolean`

`true` if position is on a greater line
or on the same line on a greater or equal character.

#### Defined in

[index.d.ts:311](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L311)

___

### isBefore

▸ **isBefore**(`other`): `boolean`

Check if this position is before `other`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](codearts_plugin_.Position.md) | A position. |

#### Returns

`boolean`

`true` if position is on a smaller line
or on the same line on a smaller character.

#### Defined in

[index.d.ts:284](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L284)

___

### isBeforeOrEqual

▸ **isBeforeOrEqual**(`other`): `boolean`

Check if this position is before or equal to `other`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](codearts_plugin_.Position.md) | A position. |

#### Returns

`boolean`

`true` if position is on a smaller line
or on the same line on a smaller or equal character.

#### Defined in

[index.d.ts:293](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L293)

___

### isEqual

▸ **isEqual**(`other`): `boolean`

Check if this position is equal to `other`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](codearts_plugin_.Position.md) | A position. |

#### Returns

`boolean`

`true` if the line and character of the given position are equal to
the line and character of this position.

#### Defined in

[index.d.ts:320](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L320)

___

### translate

▸ **translate**(`lineDelta?`, `characterDelta?`): [`Position`](codearts_plugin_.Position.md)

Create a new position relative to this position.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `lineDelta?` | `number` | Delta value for the line value, default is `0`. |
| `characterDelta?` | `number` | Delta value for the character value, default is `0`. |

#### Returns

[`Position`](codearts_plugin_.Position.md)

A position which line and character is the sum of the current line and
character and the corresponding deltas.

#### Defined in

[index.d.ts:340](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L340)

▸ **translate**(`change`): [`Position`](codearts_plugin_.Position.md)

Derived a new position relative to this position.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `change` | `Object` | An object that describes a delta to this position. |
| `change.characterDelta?` | `number` | - |
| `change.lineDelta?` | `number` | - |

#### Returns

[`Position`](codearts_plugin_.Position.md)

A position that reflects the given delta. Will return `this` position if the change
is not changing anything.

#### Defined in

[index.d.ts:349](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L349)

___

### with

▸ **with**(`line?`, `character?`): [`Position`](codearts_plugin_.Position.md)

Create a new position derived from this position.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `line?` | `number` | Value that should be used as line value, default is the [existing value](codearts_plugin_.Position.md#line) |
| `character?` | `number` | Value that should be used as character value, default is the [existing value](codearts_plugin_.Position.md#character) |

#### Returns

[`Position`](codearts_plugin_.Position.md)

A position where line and character are replaced by the given values.

#### Defined in

[index.d.ts:358](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L358)

▸ **with**(`change`): [`Position`](codearts_plugin_.Position.md)

Derived a new position from this position.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `change` | `Object` | An object that describes a change to this position. |
| `change.character?` | `number` | - |
| `change.line?` | `number` | - |

#### Returns

[`Position`](codearts_plugin_.Position.md)

A position that reflects the given change. Will return `this` position if the change
is not changing anything.

#### Defined in

[index.d.ts:367](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L367)
