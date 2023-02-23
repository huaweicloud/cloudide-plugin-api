[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Selection

# Class: Selection

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Selection

Represents a text selection in an editor.

## Hierarchy

- [`Range`](cloudide_plugin_.Range.md)

  ↳ **`Selection`**

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.Selection.md#constructor)

### Properties

- [active](cloudide_plugin_.Selection.md#active)
- [anchor](cloudide_plugin_.Selection.md#anchor)
- [end](cloudide_plugin_.Selection.md#end)
- [isEmpty](cloudide_plugin_.Selection.md#isempty)
- [isReversed](cloudide_plugin_.Selection.md#isreversed)
- [isSingleLine](cloudide_plugin_.Selection.md#issingleline)
- [start](cloudide_plugin_.Selection.md#start)

### Methods

- [contains](cloudide_plugin_.Selection.md#contains)
- [intersection](cloudide_plugin_.Selection.md#intersection)
- [isEqual](cloudide_plugin_.Selection.md#isequal)
- [union](cloudide_plugin_.Selection.md#union)
- [with](cloudide_plugin_.Selection.md#with)

## Constructors

### constructor

• **new Selection**(`anchor`, `active`)

Create a selection from two positions.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `anchor` | [`Position`](cloudide_plugin_.Position.md) | a position |
| `active` | [`Position`](cloudide_plugin_.Position.md) | a position |

#### Overrides

[Range](cloudide_plugin_.Range.md).[constructor](cloudide_plugin_.Range.md#constructor)

#### Defined in

[index.d.ts:523](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L523)

• **new Selection**(`anchorLine`, `anchorCharacter`, `activeLine`, `activeCharacter`)

Create a selection from coordinates.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `anchorLine` | `number` | a zero based line value |
| `anchorCharacter` | `number` | a zero based character value |
| `activeLine` | `number` | a zero based line value |
| `activeCharacter` | `number` | a zero based character value |

#### Overrides

[Range](cloudide_plugin_.Range.md).[constructor](cloudide_plugin_.Range.md#constructor)

#### Defined in

[index.d.ts:533](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L533)

## Properties

### active

• **active**: [`Position`](cloudide_plugin_.Position.md)

Position of the cursor

#### Defined in

[index.d.ts:510](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L510)

___

### anchor

• **anchor**: [`Position`](cloudide_plugin_.Position.md)

Position where selection starts.

#### Defined in

[index.d.ts:505](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L505)

___

### end

• `Readonly` **end**: [`Position`](cloudide_plugin_.Position.md)

End position.

#### Inherited from

[Range](cloudide_plugin_.Range.md).[end](cloudide_plugin_.Range.md#end)

#### Defined in

[index.d.ts:424](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L424)

___

### isEmpty

• **isEmpty**: `boolean`

`true` if start and end are equal

#### Inherited from

[Range](cloudide_plugin_.Range.md).[isEmpty](cloudide_plugin_.Range.md#isempty)

#### Defined in

[index.d.ts:429](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L429)

___

### isReversed

• **isReversed**: `boolean`

A selection is reversed if `active.isBefore(anchor)`

#### Defined in

[index.d.ts:515](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L515)

___

### isSingleLine

• **isSingleLine**: `boolean`

`true` if `start.line` and `end.line` are equal

#### Inherited from

[Range](cloudide_plugin_.Range.md).[isSingleLine](cloudide_plugin_.Range.md#issingleline)

#### Defined in

[index.d.ts:434](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L434)

___

### start

• `Readonly` **start**: [`Position`](cloudide_plugin_.Position.md)

Start position.

#### Inherited from

[Range](cloudide_plugin_.Range.md).[start](cloudide_plugin_.Range.md#start)

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

#### Inherited from

[Range](cloudide_plugin_.Range.md).[contains](cloudide_plugin_.Range.md#contains)

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

#### Inherited from

[Range](cloudide_plugin_.Range.md).[intersection](cloudide_plugin_.Range.md#intersection)

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

#### Inherited from

[Range](cloudide_plugin_.Range.md).[isEqual](cloudide_plugin_.Range.md#isequal)

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

#### Inherited from

[Range](cloudide_plugin_.Range.md).[union](cloudide_plugin_.Range.md#union)

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

#### Inherited from

[Range](cloudide_plugin_.Range.md).[with](cloudide_plugin_.Range.md#with)

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

#### Inherited from

[Range](cloudide_plugin_.Range.md).[with](cloudide_plugin_.Range.md#with)

#### Defined in

[index.d.ts:494](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L494)
