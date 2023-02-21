[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Range

# Class: Range

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Range

Pair of two positions.

## Hierarchy

- **`Range`**

  ↳ [`Selection`](cloudide_plugin_.Selection.md)

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.Range.md#constructor)

### Properties

- [end](cloudide_plugin_.Range.md#end)
- [isEmpty](cloudide_plugin_.Range.md#isempty)
- [isSingleLine](cloudide_plugin_.Range.md#issingleline)
- [start](cloudide_plugin_.Range.md#start)

### Methods

- [contains](cloudide_plugin_.Range.md#contains)
- [intersection](cloudide_plugin_.Range.md#intersection)
- [isEqual](cloudide_plugin_.Range.md#isequal)
- [union](cloudide_plugin_.Range.md#union)
- [with](cloudide_plugin_.Range.md#with)

## Constructors

### constructor

• **new Range**(`start`, `end`)

Create a new range from two positions.
If `start` is not before or equal to `end`, the values will be swapped.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | [`Position`](cloudide_plugin_.Position.md) | a position |
| `end` | [`Position`](cloudide_plugin_.Position.md) | a position |

#### Defined in

[index.d.ts:443](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L443)

• **new Range**(`startLine`, `startCharacter`, `endLine`, `endCharacter`)

Create a new position from coordinates.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startLine` | `number` | a zero based line value |
| `startCharacter` | `number` | a zero based character value |
| `endLine` | `number` | a zero based line value |
| `endCharacter` | `number` | a zero based character value |

#### Defined in

[index.d.ts:453](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L453)

## Properties

### end

• `Readonly` **end**: [`Position`](cloudide_plugin_.Position.md)

End position.

#### Defined in

[index.d.ts:424](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L424)

___

### isEmpty

• **isEmpty**: `boolean`

`true` if start and end are equal

#### Defined in

[index.d.ts:429](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L429)

___

### isSingleLine

• **isSingleLine**: `boolean`

`true` if `start.line` and `end.line` are equal

#### Defined in

[index.d.ts:434](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L434)

___

### start

• `Readonly` **start**: [`Position`](cloudide_plugin_.Position.md)

Start position.

#### Defined in

[index.d.ts:419](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L419)

## Methods

### contains

▸ **contains**(`positionOrRange`): `boolean`

Check if a position or a range is in this range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `positionOrRange` | [`Position`](cloudide_plugin_.Position.md) \| [`Range`](cloudide_plugin_.Range.md) | a position or a range |

#### Returns

`boolean`

#### Defined in

[index.d.ts:460](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L460)

___

### intersection

▸ **intersection**(`range`): `undefined` \| [`Range`](cloudide_plugin_.Range.md)

Intersect `range` with this range and returns new range or `undefined`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](cloudide_plugin_.Range.md) | a range |

#### Returns

`undefined` \| [`Range`](cloudide_plugin_.Range.md)

#### Defined in

[index.d.ts:474](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L474)

___

### isEqual

▸ **isEqual**(`other`): `boolean`

Check `other` equals this range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Range`](cloudide_plugin_.Range.md) | a range |

#### Returns

`boolean`

#### Defined in

[index.d.ts:467](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L467)

___

### union

▸ **union**(`other`): [`Range`](cloudide_plugin_.Range.md)

Compute the union of `other` with this range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Range`](cloudide_plugin_.Range.md) | a range |

#### Returns

[`Range`](cloudide_plugin_.Range.md)

#### Defined in

[index.d.ts:481](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L481)

___

### with

▸ **with**(`start?`, `end?`): [`Range`](cloudide_plugin_.Range.md)

Derived a new range from this range.

#### Parameters

| Name | Type |
| :------ | :------ |
| `start?` | [`Position`](cloudide_plugin_.Position.md) |
| `end?` | [`Position`](cloudide_plugin_.Position.md) |

#### Returns

[`Range`](cloudide_plugin_.Range.md)

#### Defined in

[index.d.ts:489](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L489)

▸ **with**(`change`): [`Range`](cloudide_plugin_.Range.md)

Derived a new range from this range.

#### Parameters

| Name | Type |
| :------ | :------ |
| `change` | `Object` |
| `change.end?` | [`Position`](cloudide_plugin_.Position.md) |
| `change.start?` | [`Position`](cloudide_plugin_.Position.md) |

#### Returns

[`Range`](cloudide_plugin_.Range.md)

#### Defined in

[index.d.ts:494](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L494)
