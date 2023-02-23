[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / InputBox

# Interface: InputBox

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).InputBox

A concrete [QuickInput](#QuickInput) to let the user input a text value.

Note that in many cases the more convenient [window.showInputBox](#window.showInputBox)
is easier to use. [window.createInputBox](#window.createInputBox) should be used
when [window.showInputBox](#window.showInputBox) does not offer the required flexibility.

## Hierarchy

- [`QuickInput`](cloudide_plugin_.QuickInput.md)

  ↳ **`InputBox`**

## Table of contents

### Properties

- [busy](cloudide_plugin_.InputBox.md#busy)
- [buttons](cloudide_plugin_.InputBox.md#buttons)
- [enabled](cloudide_plugin_.InputBox.md#enabled)
- [ignoreFocusOut](cloudide_plugin_.InputBox.md#ignorefocusout)
- [onDidAccept](cloudide_plugin_.InputBox.md#ondidaccept)
- [onDidChangeValue](cloudide_plugin_.InputBox.md#ondidchangevalue)
- [onDidHide](cloudide_plugin_.InputBox.md#ondidhide)
- [onDidTriggerButton](cloudide_plugin_.InputBox.md#ondidtriggerbutton)
- [password](cloudide_plugin_.InputBox.md#password)
- [placeholder](cloudide_plugin_.InputBox.md#placeholder)
- [prompt](cloudide_plugin_.InputBox.md#prompt)
- [step](cloudide_plugin_.InputBox.md#step)
- [title](cloudide_plugin_.InputBox.md#title)
- [totalSteps](cloudide_plugin_.InputBox.md#totalsteps)
- [validationMessage](cloudide_plugin_.InputBox.md#validationmessage)
- [value](cloudide_plugin_.InputBox.md#value)

### Methods

- [dispose](cloudide_plugin_.InputBox.md#dispose)
- [hide](cloudide_plugin_.InputBox.md#hide)
- [show](cloudide_plugin_.InputBox.md#show)

## Properties

### busy

• **busy**: `boolean`

If the UI should show a progress indicator. Defaults to false.

Change this to true, e.g., while loading more data or validating
user input.

#### Inherited from

[QuickInput](cloudide_plugin_.QuickInput.md).[busy](cloudide_plugin_.QuickInput.md#busy)

#### Defined in

[index.d.ts:5046](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5046)

___

### buttons

• **buttons**: readonly [`QuickInputButton`](cloudide_plugin_.QuickInputButton.md)[]

Buttons for actions in the UI.

#### Defined in

[index.d.ts:4976](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4976)

___

### enabled

• **enabled**: `boolean`

If the UI should allow for user input. Defaults to true.

Change this to false, e.g., while validating user input or
loading data for the next step in user input.

#### Inherited from

[QuickInput](cloudide_plugin_.QuickInput.md).[enabled](cloudide_plugin_.QuickInput.md#enabled)

#### Defined in

[index.d.ts:5038](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5038)

___

### ignoreFocusOut

• **ignoreFocusOut**: `boolean`

If the UI should stay open even when loosing UI focus. Defaults to false.

#### Inherited from

[QuickInput](cloudide_plugin_.QuickInput.md).[ignoreFocusOut](cloudide_plugin_.QuickInput.md#ignorefocusout)

#### Defined in

[index.d.ts:5051](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5051)

___

### onDidAccept

• `Readonly` **onDidAccept**: [`Event`](cloudide_plugin_.Event.md)<`void`\>

An event signaling when the user indicated acceptance of the input value.

#### Defined in

[index.d.ts:4971](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4971)

___

### onDidChangeValue

• `Readonly` **onDidChangeValue**: [`Event`](cloudide_plugin_.Event.md)<`string`\>

An event signaling when the value has changed.

#### Defined in

[index.d.ts:4966](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4966)

___

### onDidHide

• **onDidHide**: [`Event`](cloudide_plugin_.Event.md)<`void`\>

An event signaling when this input UI is hidden.

There are several reasons why this UI might have to be hidden and
the extension will be notified through [QuickInput.onDidHide](#QuickInput.onDidHide).
(Examples include: an explicit call to [QuickInput.hide](#QuickInput.hide),
the user pressing Esc, some other input UI opening, etc.)

#### Inherited from

[QuickInput](cloudide_plugin_.QuickInput.md).[onDidHide](cloudide_plugin_.QuickInput.md#ondidhide)

#### Defined in

[index.d.ts:5073](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5073)

___

### onDidTriggerButton

• `Readonly` **onDidTriggerButton**: [`Event`](cloudide_plugin_.Event.md)<[`QuickInputButton`](cloudide_plugin_.QuickInputButton.md)\>

An event signaling when a button was triggered.

#### Defined in

[index.d.ts:4981](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4981)

___

### password

• **password**: `boolean`

If the input value should be hidden. Defaults to false.

#### Defined in

[index.d.ts:4961](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4961)

___

### placeholder

• **placeholder**: `undefined` \| `string`

Optional placeholder in the filter text.

#### Defined in

[index.d.ts:4956](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4956)

___

### prompt

• **prompt**: `undefined` \| `string`

An optional prompt text providing some ask or explanation to the user.

#### Defined in

[index.d.ts:4986](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4986)

___

### step

• **step**: `undefined` \| `number`

An optional current step count.

#### Inherited from

[QuickInput](cloudide_plugin_.QuickInput.md).[step](cloudide_plugin_.QuickInput.md#step)

#### Defined in

[index.d.ts:5025](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5025)

___

### title

• **title**: `undefined` \| `string`

An optional title.

#### Inherited from

[QuickInput](cloudide_plugin_.QuickInput.md).[title](cloudide_plugin_.QuickInput.md#title)

#### Defined in

[index.d.ts:5020](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5020)

___

### totalSteps

• **totalSteps**: `undefined` \| `number`

An optional total step count.

#### Inherited from

[QuickInput](cloudide_plugin_.QuickInput.md).[totalSteps](cloudide_plugin_.QuickInput.md#totalsteps)

#### Defined in

[index.d.ts:5030](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5030)

___

### validationMessage

• **validationMessage**: `undefined` \| `string`

An optional validation message indicating a problem with the current input value.

#### Defined in

[index.d.ts:4991](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4991)

___

### value

• **value**: `string`

Current input value.

#### Defined in

[index.d.ts:4951](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L4951)

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

[QuickInput](cloudide_plugin_.QuickInput.md).[dispose](cloudide_plugin_.QuickInput.md#dispose)

#### Defined in

[index.d.ts:5081](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5081)

___

### hide

▸ **hide**(): `void`

Hides this input UI. This will also fire an [QuickInput.onDidHide](#QuickInput.onDidHide)
event.

#### Returns

`void`

#### Inherited from

[QuickInput](cloudide_plugin_.QuickInput.md).[hide](cloudide_plugin_.QuickInput.md#hide)

#### Defined in

[index.d.ts:5063](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5063)

___

### show

▸ **show**(): `void`

Makes the input UI visible in its current configuration. Any other input
UI will first fire an [QuickInput.onDidHide](#QuickInput.onDidHide) event.

#### Returns

`void`

#### Inherited from

[QuickInput](cloudide_plugin_.QuickInput.md).[show](cloudide_plugin_.QuickInput.md#show)

#### Defined in

[index.d.ts:5057](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5057)
