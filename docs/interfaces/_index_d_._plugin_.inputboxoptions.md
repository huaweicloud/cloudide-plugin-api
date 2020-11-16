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

*Defined in [index.d.ts:1846](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1846)*

Set to `true` to keep the input box open when focus moves to another part of the editor or to another window.

___

### password

• `Optional` **password**: boolean

*Defined in [index.d.ts:1841](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1841)*

Controls if a password input is shown. Password input hides the typed text.

___

### placeHolder

• `Optional` **placeHolder**: string

*Defined in [index.d.ts:1836](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1836)*

An optional string to show as placeholder in the input box to guide the user what to type.

___

### prompt

• `Optional` **prompt**: string

*Defined in [index.d.ts:1831](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1831)*

The text to display underneath the input box.

___

### value

• `Optional` **value**: string

*Defined in [index.d.ts:1818](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1818)*

The value to prefill in the input box.

___

### valueSelection

• `Optional` **valueSelection**: [number, number]

*Defined in [index.d.ts:1826](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1826)*

Selection of the prefilled [`value`](#InputBoxOptions.value). Defined as tuple of two number where the
first is the inclusive start index and the second the exclusive end index. When `undefined` the whole
word will be selected, when empty (start equals end) only the cursor will be set,
otherwise the defined range will be selected.

## Methods

### validateInput

▸ `Optional`**validateInput**(`value`: string): string \| undefined \| null \| [Thenable](_index_d_.thenable.md)\<string \| undefined \| null>

*Defined in [index.d.ts:1856](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1856)*

An optional function that will be called to validate input and to give a hint
to the user.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`value` | string | The current value of the input box. |

**Returns:** string \| undefined \| null \| [Thenable](_index_d_.thenable.md)\<string \| undefined \| null>

A human-readable string which is presented as diagnostic message.
Return `undefined`, `null`, or the empty string when 'value' is valid.
