**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / InputBoxOptions

# Interface: InputBoxOptions

Options to configure the behavior of the input box UI.

## Hierarchy

* **InputBoxOptions**

## Index

### Properties

* [ignoreFocusOut](_index_d_._plugin_.inputboxoptions.md#ignorefocusout)
* [password](_index_d_._plugin_.inputboxoptions.md#password)
* [placeHolder](_index_d_._plugin_.inputboxoptions.md#placeholder)
* [prompt](_index_d_._plugin_.inputboxoptions.md#prompt)
* [value](_index_d_._plugin_.inputboxoptions.md#value)
* [valueSelection](_index_d_._plugin_.inputboxoptions.md#valueselection)

### Methods

* [validateInput](_index_d_._plugin_.inputboxoptions.md#validateinput)

## Properties

### ignoreFocusOut

• `Optional` **ignoreFocusOut**: boolean

*Defined in [index.d.ts:1999](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1999)*

Set to `true` to keep the input box open when focus moves to another part of the editor or to another window.

___

### password

• `Optional` **password**: boolean

*Defined in [index.d.ts:1994](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1994)*

Controls if a password input is shown. Password input hides the typed text.

___

### placeHolder

• `Optional` **placeHolder**: string

*Defined in [index.d.ts:1989](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1989)*

An optional string to show as placeholder in the input box to guide the user what to type.

___

### prompt

• `Optional` **prompt**: string

*Defined in [index.d.ts:1984](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1984)*

The text to display underneath the input box.

___

### value

• `Optional` **value**: string

*Defined in [index.d.ts:1971](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1971)*

The value to prefill in the input box.

___

### valueSelection

• `Optional` **valueSelection**: [number, number]

*Defined in [index.d.ts:1979](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1979)*

Selection of the prefilled [`value`](#InputBoxOptions.value). Defined as tuple of two number where the
first is the inclusive start index and the second the exclusive end index. When `undefined` the whole
word will be selected, when empty (start equals end) only the cursor will be set,
otherwise the defined range will be selected.

## Methods

### validateInput

▸ `Optional`**validateInput**(`value`: string): string \| undefined \| null \| [Thenable](_index_d_.thenable.md)\<string \| undefined \| null>

*Defined in [index.d.ts:2009](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2009)*

An optional function that will be called to validate input and to give a hint
to the user.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`value` | string | The current value of the input box. |

**Returns:** string \| undefined \| null \| [Thenable](_index_d_.thenable.md)\<string \| undefined \| null>

A human-readable string which is presented as diagnostic message.
Return `undefined`, `null`, or the empty string when 'value' is valid.
