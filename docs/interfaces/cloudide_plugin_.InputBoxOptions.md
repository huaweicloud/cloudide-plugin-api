[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / InputBoxOptions

# Interface: InputBoxOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).InputBoxOptions

Options to configure the behavior of the input box UI.

## Table of contents

### Properties

- [ignoreFocusOut](cloudide_plugin_.InputBoxOptions.md#ignorefocusout)
- [password](cloudide_plugin_.InputBoxOptions.md#password)
- [placeHolder](cloudide_plugin_.InputBoxOptions.md#placeholder)
- [prompt](cloudide_plugin_.InputBoxOptions.md#prompt)
- [validateInput](cloudide_plugin_.InputBoxOptions.md#validateinput)
- [value](cloudide_plugin_.InputBoxOptions.md#value)
- [valueSelection](cloudide_plugin_.InputBoxOptions.md#valueselection)

### Methods

- [onAccept](cloudide_plugin_.InputBoxOptions.md#onaccept)

## Properties

### ignoreFocusOut

• `Optional` **ignoreFocusOut**: `boolean`

Set to `true` to keep the input box open when focus moves to another part of the editor or to another window.

#### Defined in

[index.d.ts:2352](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2352)

___

### password

• `Optional` **password**: `boolean`

Set to `true` to show a password prompt that will not show the typed value.

#### Defined in

[index.d.ts:2347](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2347)

___

### placeHolder

• `Optional` **placeHolder**: `string`

An optional string to show as place holder in the input box to guide the user what to type.

#### Defined in

[index.d.ts:2342](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2342)

___

### prompt

• `Optional` **prompt**: `string`

The text to display underneath the input box.

#### Defined in

[index.d.ts:2337](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2337)

___

### validateInput

• `Optional` **validateInput**: (`input`: `string`) => `undefined` \| `Promise`<`undefined` \| ``null`` \| `string`\>

#### Type declaration

▸ (`input`): `undefined` \| `Promise`<`undefined` \| ``null`` \| `string`\>

An optional function that will be called to validate input and to give a hint
to the user.

##### Parameters

| Name | Type |
| :------ | :------ |
| `input` | `string` |

##### Returns

`undefined` \| `Promise`<`undefined` \| ``null`` \| `string`\>

A human readable string which is presented as diagnostic message.
Return `undefined`, or the empty string when 'value' is valid.

#### Defined in

[index.d.ts:2362](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2362)

___

### value

• `Optional` **value**: `string`

The value to prefill in the input box.

#### Defined in

[index.d.ts:2324](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2324)

___

### valueSelection

• `Optional` **valueSelection**: [`number`, `number`]

Selection of the prefilled [`value`](#InputBoxOptions.value). Defined as tuple of two number where the
first is the inclusive start index and the second the exclusive end index. When `undefined` the whole
word will be selected, when empty (start equals end) only the cursor will be set,
otherwise the defined range will be selected.

#### Defined in

[index.d.ts:2332](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2332)

## Methods

### onAccept

▸ `Optional` **onAccept**(): `void`

An optional function that will be called on Enter key.

#### Returns

`void`

#### Defined in

[index.d.ts:2367](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2367)
