[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TreeViewEditBoxOptions

# Interface: TreeViewEditBoxOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).TreeViewEditBoxOptions

## Table of contents

### Properties

- [placeholder](codearts_plugin_.TreeViewEditBoxOptions.md#placeholder)
- [validateInput](codearts_plugin_.TreeViewEditBoxOptions.md#validateinput)
- [value](codearts_plugin_.TreeViewEditBoxOptions.md#value)
- [valueSelection](codearts_plugin_.TreeViewEditBoxOptions.md#valueselection)

## Properties

### placeholder

• `Optional` **placeholder**: `string`

An optional string to show as placeholder in the input box to guide the user what to type.

#### Defined in

[index.d.ts:10956](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10956)

___

### validateInput

• `Optional` **validateInput**: (`value`: `string`, `isAcceptEvent`: `boolean`) => `undefined` \| ``null`` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md) \| [`Thenable`](Thenable.md)<`undefined` \| ``null`` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md)\>

#### Type declaration

▸ (`value`, `isAcceptEvent`): `undefined` \| ``null`` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md) \| [`Thenable`](Thenable.md)<`undefined` \| ``null`` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md)\>

An optional function that will be called to validate input and to give a hint
to the user.

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | The current value of the input box. |
| `isAcceptEvent` | `boolean` | Whether this validation is triggered by the accept or change event. |

##### Returns

`undefined` \| ``null`` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md) \| [`Thenable`](Thenable.md)<`undefined` \| ``null`` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md)\>

[InputBoxValidationMessage](codearts_plugin_.InputBoxValidationMessage.md) which can provide a specific message severity.
  Return `undefined`, `null`, or the empty string when 'value' is valid.

#### Defined in

[index.d.ts:10980](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10980)

___

### value

• `Optional` **value**: `string`

The value to prefill in the input box.

#### Defined in

[index.d.ts:10961](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10961)

___

### valueSelection

• `Optional` **valueSelection**: [`number`, `number`]

Selection of the prefilled [`value`](#TreeViewEditBoxOptions.value). Defined as tuple of two number where the
first is the inclusive start index and the second the exclusive end index. When `undefined` the whole
word will be selected, when empty (start equals end) only the cursor will be set,
otherwise the defined range will be selected.

#### Defined in

[index.d.ts:10969](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L10969)
