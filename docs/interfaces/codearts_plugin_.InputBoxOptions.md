[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InputBoxOptions

# Interface: InputBoxOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).InputBoxOptions

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

#### Defined in

[index.d.ts:2054](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L2054)

___

### password

• `Optional` **password**: `boolean`

#### Defined in

[index.d.ts:2048](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L2048)

___

### placeHolder

• `Optional` **placeHolder**: `string`

#### Defined in

[index.d.ts:2043](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L2043)

___

### prompt

• `Optional` **prompt**: `string`

#### Defined in

[index.d.ts:2038](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L2038)

___

### title

• `Optional` **title**: `string`

#### Defined in

[index.d.ts:2020](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L2020)

___

### value

• `Optional` **value**: `string`

#### Defined in

[index.d.ts:2025](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L2025)

___

### valueSelection

• `Optional` **valueSelection**: [`number`, `number`]

#### Defined in

[index.d.ts:2033](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L2033)

## Methods

### validateInput

▸ `Optional` **validateInput**(`value`): `undefined` \| ``null`` \| `string` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md) \| [`Thenable`](Thenable.md)<`undefined` \| ``null`` \| `string` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` |  |

#### Returns

`undefined` \| ``null`` \| `string` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md) \| [`Thenable`](Thenable.md)<`undefined` \| ``null`` \| `string` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md)\>

#### Defined in

[index.d.ts:2064](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L2064)
