[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InputBox

# Interface: InputBox

["@codearts/plugin"](../modules/_codearts_plugin_.md).InputBox

A concrete [QuickInput](codearts_plugin_.QuickInput.md) to let the user input a text value.

Note that in many cases the more convenient [showInputBox](../modules/codearts_plugin_.window.md#showinputbox)
is easier to use. [createInputBox](../modules/codearts_plugin_.window.md#createinputbox) should be used
when [showInputBox](../modules/codearts_plugin_.window.md#showinputbox) does not offer the required flexibility.

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

If the UI should show a progress indicator. Defaults to false.

Change this to true, e.g., while loading more data or validating
user input.

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[busy](codearts_plugin_.QuickInput.md#busy)

#### Defined in

[index.d.ts:11043](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11043)

___

### buttons

• **buttons**: readonly [`QuickInputButton`](codearts_plugin_.QuickInputButton.md)[]

Buttons for actions in the UI.

#### Defined in

[index.d.ts:11214](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11214)

___

### enabled

• **enabled**: `boolean`

If the UI should allow for user input. Defaults to true.

Change this to false, e.g., while validating user input or
loading data for the next step in user input.

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[enabled](codearts_plugin_.QuickInput.md#enabled)

#### Defined in

[index.d.ts:11035](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11035)

___

### ignoreFocusOut

• **ignoreFocusOut**: `boolean`

If the UI should stay open even when loosing UI focus. Defaults to false.
This setting is ignored on iPad and is always false.

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[ignoreFocusOut](codearts_plugin_.QuickInput.md#ignorefocusout)

#### Defined in

[index.d.ts:11049](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11049)

___

### onDidAccept

• `Readonly` **onDidAccept**: [`Event`](codearts_plugin_.Event.md)<`void`\>

An event signaling when the user indicated acceptance of the input value.

#### Defined in

[index.d.ts:11209](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11209)

___

### onDidChangeValue

• `Readonly` **onDidChangeValue**: [`Event`](codearts_plugin_.Event.md)<`string`\>

An event signaling when the value has changed.

#### Defined in

[index.d.ts:11204](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11204)

___

### onDidHide

• **onDidHide**: [`Event`](codearts_plugin_.Event.md)<`void`\>

An event signaling when this input UI is hidden.

There are several reasons why this UI might have to be hidden and
the extension will be notified through [onDidHide](codearts_plugin_.QuickInput.md#ondidhide).
(Examples include: an explicit call to [hide](codearts_plugin_.QuickInput.md#hide),
the user pressing Esc, some other input UI opening, etc.)

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[onDidHide](codearts_plugin_.QuickInput.md#ondidhide)

#### Defined in

[index.d.ts:11071](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11071)

___

### onDidTriggerButton

• `Readonly` **onDidTriggerButton**: [`Event`](codearts_plugin_.Event.md)<[`QuickInputButton`](codearts_plugin_.QuickInputButton.md)\>

An event signaling when a button was triggered.

#### Defined in

[index.d.ts:11219](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11219)

___

### password

• **password**: `boolean`

If the input value should be hidden. Defaults to false.

#### Defined in

[index.d.ts:11199](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11199)

___

### placeholder

• **placeholder**: `undefined` \| `string`

Optional placeholder in the filter text.

#### Defined in

[index.d.ts:11194](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11194)

___

### prompt

• **prompt**: `undefined` \| `string`

An optional prompt text providing some ask or explanation to the user.

#### Defined in

[index.d.ts:11224](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11224)

___

### step

• **step**: `undefined` \| `number`

An optional current step count.

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[step](codearts_plugin_.QuickInput.md#step)

#### Defined in

[index.d.ts:11022](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11022)

___

### title

• **title**: `undefined` \| `string`

An optional title.

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[title](codearts_plugin_.QuickInput.md#title)

#### Defined in

[index.d.ts:11017](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11017)

___

### totalSteps

• **totalSteps**: `undefined` \| `number`

An optional total step count.

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[totalSteps](codearts_plugin_.QuickInput.md#totalsteps)

#### Defined in

[index.d.ts:11027](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11027)

___

### validationMessage

• **validationMessage**: `undefined` \| `string` \| [`InputBoxValidationMessage`](codearts_plugin_.InputBoxValidationMessage.md)

An optional validation message indicating a problem with the current input value.
By returning a string, the InputBox will use a default [InputBoxValidationSeverity](../enums/codearts_plugin_.InputBoxValidationSeverity.md) of Error.
Returning undefined clears the validation message.

#### Defined in

[index.d.ts:11231](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11231)

___

### value

• **value**: `string`

Current input value.

#### Defined in

[index.d.ts:11189](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11189)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose of this input UI and any associated resources. If it is still
visible, it is first hidden. After this call the input UI is no longer
functional and no additional methods or properties on it should be
accessed. Instead a new input UI should be created.

#### Returns

`void`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[dispose](codearts_plugin_.QuickInput.md#dispose)

#### Defined in

[index.d.ts:11079](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11079)

___

### hide

▸ **hide**(): `void`

Hides this input UI. This will also fire an [onDidHide](codearts_plugin_.QuickInput.md#ondidhide)
event.

#### Returns

`void`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[hide](codearts_plugin_.QuickInput.md#hide)

#### Defined in

[index.d.ts:11061](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11061)

___

### show

▸ **show**(): `void`

Makes the input UI visible in its current configuration. Any other input
UI will first fire an [onDidHide](codearts_plugin_.QuickInput.md#ondidhide) event.

#### Returns

`void`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[show](codearts_plugin_.QuickInput.md#show)

#### Defined in

[index.d.ts:11055](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11055)
