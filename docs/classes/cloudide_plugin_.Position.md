[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Position

# Class: Position

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Position

Represents a line and character position.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.Position.md#constructor)

### Properties

- [character](cloudide_plugin_.Position.md#character)
- [line](cloudide_plugin_.Position.md#line)

### Methods

- [compareTo](cloudide_plugin_.Position.md#compareto)
- [isAfter](cloudide_plugin_.Position.md#isafter)
- [isAfterOrEqual](cloudide_plugin_.Position.md#isafterorequal)
- [isBefore](cloudide_plugin_.Position.md#isbefore)
- [isBeforeOrEqual](cloudide_plugin_.Position.md#isbeforeorequal)
- [isEqual](cloudide_plugin_.Position.md#isequal)
- [translate](cloudide_plugin_.Position.md#translate)
- [with](cloudide_plugin_.Position.md#with)

## Constructors

### constructor

• **new Position**(`line`, `character`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `line` | `number` |
| `character` | `number` |

#### Defined in

[index.d.ts:317](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L317)

## Properties

### character

• `Readonly` **character**: `number`

The zero-based character value.

#### Defined in

[index.d.ts:315](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L315)

___

### line

• `Readonly` **line**: `number`

The zero-based line value.

#### Defined in

[index.d.ts:310](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L310)

## Methods

### compareTo

▸ **compareTo**(`other`): `number`

Compare this to `other`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](cloudide_plugin_.Position.md) | A position. |

#### Returns

`number`

A number smaller than zero if this position is before the given position,
a number greater than zero if this position is after the given position, or zero when
this and the given position are equal.

#### Defined in

[index.d.ts:372](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L372)

___

### isAfter

▸ **isAfter**(`other`): `boolean`

Check if this position is after `other`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](cloudide_plugin_.Position.md) | A position. |

#### Returns

`boolean`

`true` if position is on a greater line
or on the same line on a greater character.

#### Defined in

[index.d.ts:344](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L344)

___

### isAfterOrEqual

▸ **isAfterOrEqual**(`other`): `boolean`

Check if this position is after or equal to `other`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](cloudide_plugin_.Position.md) | A position. |

#### Returns

`boolean`

`true` if position is on a greater line
or on the same line on a greater or equal character.

#### Defined in

[index.d.ts:353](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L353)

___

### isBefore

▸ **isBefore**(`other`): `boolean`

Check if this position is before `other`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](cloudide_plugin_.Position.md) | A position. |

#### Returns

`boolean`

`true` if position is on a smaller line
or on the same line on a smaller character.

#### Defined in

[index.d.ts:326](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L326)

___

### isBeforeOrEqual

▸ **isBeforeOrEqual**(`other`): `boolean`

Check if this position is before or equal to `other`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](cloudide_plugin_.Position.md) | A position. |

#### Returns

`boolean`

`true` if position is on a smaller line
or on the same line on a smaller or equal character.

#### Defined in

[index.d.ts:335](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L335)

___

### isEqual

▸ **isEqual**(`other`): `boolean`

Check if this position is equal to `other`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Position`](cloudide_plugin_.Position.md) | A position. |

#### Returns

`boolean`

`true` if the line and character of the given position are equal to
the line and character of this position.

#### Defined in

[index.d.ts:362](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L362)

___

### translate

▸ **translate**(`lineDelta?`, `characterDelta?`): [`Position`](cloudide_plugin_.Position.md)

Create a new position relative to this position.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `lineDelta?` | `number` | Delta value for the line value, default is `0`. |
| `characterDelta?` | `number` | Delta value for the character value, default is `0`. |

#### Returns

[`Position`](cloudide_plugin_.Position.md)

A position which line and character is the sum of the current line and
character and the corresponding deltas.

#### Defined in

[index.d.ts:382](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L382)

▸ **translate**(`change`): [`Position`](cloudide_plugin_.Position.md)

Derived a new position relative to this position.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `change` | `Object` | An object that describes a delta to this position. |
| `change.characterDelta?` | `number` | - |
| `change.lineDelta?` | `number` | - |

#### Returns

[`Position`](cloudide_plugin_.Position.md)

A position that reflects the given delta. Will return `this` position if the change
is not changing anything.

#### Defined in

[index.d.ts:391](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L391)

___

### with

▸ **with**(`line?`, `character?`): [`Position`](cloudide_plugin_.Position.md)

Create a new position derived from this position.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `line?` | `number` | Value that should be used as line value, default is the [existing value](#Position.line) |
| `character?` | `number` | Value that should be used as character value, default is the [existing value](#Position.character) |

#### Returns

[`Position`](cloudide_plugin_.Position.md)

A position where line and character are replaced by the given values.

#### Defined in

[index.d.ts:400](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L400)

▸ **with**(`change`): [`Position`](cloudide_plugin_.Position.md)

Derived a new position from this position.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `change` | `Object` | An object that describes a change to this position. |
| `change.character?` | `number` | - |
| `change.line?` | `number` | - |

#### Returns

[`Position`](cloudide_plugin_.Position.md)

A position that reflects the given change. Will return `this` position if the change
is not changing anything.

#### Defined in

[index.d.ts:409](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L409)
