[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InputBoxOptions

# Interface: InputBoxOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).InputBoxOptions

Options to configure the behavior of the input box UI.

## Table of contents

### Properties

- [ignoreFocusOut](codearts_plugin_.InputBoxOptions.md#ignorefocusout)
- [password](codearts_plugin_.InputBoxOptions.md#password)
- [placeHolder](codearts_plugin_.InputBoxOptions.md#placeholder)
- [prompt](codearts_plugin_.InputBoxOptions.md#prompt)
- [title](codearts_plugin_.InputBoxOptions.md#title)
- [value](codearts_plugin_.InputBoxOptions.md#value)
- [valueSelection](codearts_plugin_.InputBoxOptions.md#valueselection)

### Methods

- [validateInput](codearts_plugin_.InputBoxOptions.md#validateinput)

## Properties

### ignoreFocusOut

• `Optional` **ignoreFocusOut**: `boolean`

Set to `true` to keep the input box open when focus moves to another part of the editor or to another window.
This setting is ignored on iPad and is always false.

#### Defined in

[index.d.ts:2054](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2054)

___

### password

• `Optional` **password**: `boolean`

Controls if a password input is shown. Password input hides the typed text.

#### Defined in

[index.d.ts:2048](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2048)

___

### placeHolder

• `Optional` **placeHolder**: `string`

An optional string to show as placeholder in the input box to guide the user what to type.

#### Defined in

[index.d.ts:2043](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2043)

___

### prompt

• `Optional` **prompt**: `string`

The text to display underneath the input box.

#### Defined in

[index.d.ts:2038](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2038)

___

### title

• `Optional` **title**: `string`

An optional string that represents the title of the input box.

#### Defined in

[index.d.ts:2020](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2020)

___

### value

• `Optional` **value**: `string`

The value to pre-fill in the input box.

#### Defined in

[index.d.ts:2025](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2025)

___

### valueSelection

• `Optional` **valueSelection**: [`number`, `number`]

Selection of the pre-filled [`value`](codearts_plugin_.InputBoxOptions.md#value). Defined as tuple of two number where the
first is the inclusive start index and the second the exclusive end index. When `undefined` the whole
word will be selected, when empty (start equals end) only the cursor will be set,
otherwise the defined range will be selected.

#### Defined in

[index.d.ts:2033](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2033)

## Methods

### validateInput

▸ `Optional` **validateInput**(`value`): `undefined` \| ``null`` \| `string` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md) \| [`Thenable`](Thenable.md)<`undefined` \| ``null`` \| `string` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md)\>

An optional function that will be called to validate input and to give a hint
to the user.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | The current value of the input box. |

#### Returns

`undefined` \| ``null`` \| `string` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md) \| [`Thenable`](Thenable.md)<`undefined` \| ``null`` \| `string` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md)\>

Either a human-readable string which is presented as an error message or an [InputBoxValidationMessage](codearts_plugin_.InputBoxValidationMessage.md)
 which can provide a specific message severity. Return `undefined`, `null`, or the empty string when 'value' is valid.

#### Defined in

[index.d.ts:2064](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2064)
