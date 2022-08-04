[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InputBox

# Interface: InputBox

["@codearts/plugin"](../modules/_codearts_plugin_.md).InputBox

## Hierarchy

- [`QuickInput`](codearts_plugin_.QuickInput.md)

  ↳ **`InputBox`**

## Table of contents

### Properties

- [busy](codearts_plugin_.InputBox.md#busy)
- [buttons](codearts_plugin_.InputBox.md#buttons)
- [enabled](codearts_plugin_.InputBox.md#enabled)
- [ignoreFocusOut](codearts_plugin_.InputBox.md#ignorefocusout)
- [onDidAccept](codearts_plugin_.InputBox.md#ondidaccept)
- [onDidChangeValue](codearts_plugin_.InputBox.md#ondidchangevalue)
- [onDidHide](codearts_plugin_.InputBox.md#ondidhide)
- [onDidTriggerButton](codearts_plugin_.InputBox.md#ondidtriggerbutton)
- [password](codearts_plugin_.InputBox.md#password)
- [placeholder](codearts_plugin_.InputBox.md#placeholder)
- [prompt](codearts_plugin_.InputBox.md#prompt)
- [step](codearts_plugin_.InputBox.md#step)
- [title](codearts_plugin_.InputBox.md#title)
- [totalSteps](codearts_plugin_.InputBox.md#totalsteps)
- [validationMessage](codearts_plugin_.InputBox.md#validationmessage)
- [value](codearts_plugin_.InputBox.md#value)

### Methods

- [dispose](codearts_plugin_.InputBox.md#dispose)
- [hide](codearts_plugin_.InputBox.md#hide)
- [show](codearts_plugin_.InputBox.md#show)

## Properties

### busy

• **busy**: `boolean`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[busy](codearts_plugin_.QuickInput.md#busy)

#### Defined in

[index.d.ts:10981](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10981)

___

### buttons

• **buttons**: readonly [`QuickInputButton`](codearts_plugin_.QuickInputButton.md)[]

#### Defined in

[index.d.ts:11152](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11152)

___

### enabled

• **enabled**: `boolean`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[enabled](codearts_plugin_.QuickInput.md#enabled)

#### Defined in

[index.d.ts:10973](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10973)

___

### ignoreFocusOut

• **ignoreFocusOut**: `boolean`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[ignoreFocusOut](codearts_plugin_.QuickInput.md#ignorefocusout)

#### Defined in

[index.d.ts:10987](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10987)

___

### onDidAccept

• `Readonly` **onDidAccept**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Defined in

[index.d.ts:11147](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11147)

___

### onDidChangeValue

• `Readonly` **onDidChangeValue**: [`Event`](codearts_plugin_.Event.md)<`string`\>

#### Defined in

[index.d.ts:11142](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11142)

___

### onDidHide

• **onDidHide**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[onDidHide](codearts_plugin_.QuickInput.md#ondidhide)

#### Defined in

[index.d.ts:11009](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11009)

___

### onDidTriggerButton

• `Readonly` **onDidTriggerButton**: [`Event`](codearts_plugin_.Event.md)<[`QuickInputButton`](codearts_plugin_.QuickInputButton.md)\>

#### Defined in

[index.d.ts:11157](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11157)

___

### password

• **password**: `boolean`

#### Defined in

[index.d.ts:11137](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11137)

___

### placeholder

• **placeholder**: `undefined` \| `string`

#### Defined in

[index.d.ts:11132](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11132)

___

### prompt

• **prompt**: `undefined` \| `string`

#### Defined in

[index.d.ts:11162](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11162)

___

### step

• **step**: `undefined` \| `number`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[step](codearts_plugin_.QuickInput.md#step)

#### Defined in

[index.d.ts:10960](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10960)

___

### title

• **title**: `undefined` \| `string`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[title](codearts_plugin_.QuickInput.md#title)

#### Defined in

[index.d.ts:10955](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10955)

___

### totalSteps

• **totalSteps**: `undefined` \| `number`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[totalSteps](codearts_plugin_.QuickInput.md#totalsteps)

#### Defined in

[index.d.ts:10965](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10965)

___

### validationMessage

• **validationMessage**: `undefined` \| `string` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md)

#### Defined in

[index.d.ts:11169](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11169)

___

### value

• **value**: `string`

#### Defined in

[index.d.ts:11127](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11127)

## Methods

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[dispose](codearts_plugin_.QuickInput.md#dispose)

#### Defined in

[index.d.ts:11017](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L11017)

___

### hide

▸ **hide**(): `void`

#### Returns

`void`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[hide](codearts_plugin_.QuickInput.md#hide)

#### Defined in

[index.d.ts:10999](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10999)

___

### show

▸ **show**(): `void`

#### Returns

`void`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[show](codearts_plugin_.QuickInput.md#show)

#### Defined in

[index.d.ts:10993](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L10993)
