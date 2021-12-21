**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / InputBox

# Interface: InputBox

A concrete [QuickInput](#QuickInput) to let the user input a text value.

Note that in many cases the more convenient [window.showInputBox](#window.showInputBox)
is easier to use. [window.createInputBox](#window.createInputBox) should be used
when [window.showInputBox](#window.showInputBox) does not offer the required flexibility.

## Hierarchy

* [QuickInput](_index_d_._plugin_.quickinput.md)

  ↳ **InputBox**

## Index

### Properties

* [busy](_index_d_._plugin_.inputbox.md#busy)
* [buttons](_index_d_._plugin_.inputbox.md#buttons)
* [enabled](_index_d_._plugin_.inputbox.md#enabled)
* [ignoreFocusOut](_index_d_._plugin_.inputbox.md#ignorefocusout)
* [onDidAccept](_index_d_._plugin_.inputbox.md#ondidaccept)
* [onDidChangeValue](_index_d_._plugin_.inputbox.md#ondidchangevalue)
* [onDidHide](_index_d_._plugin_.inputbox.md#ondidhide)
* [onDidTriggerButton](_index_d_._plugin_.inputbox.md#ondidtriggerbutton)
* [password](_index_d_._plugin_.inputbox.md#password)
* [placeholder](_index_d_._plugin_.inputbox.md#placeholder)
* [prompt](_index_d_._plugin_.inputbox.md#prompt)
* [step](_index_d_._plugin_.inputbox.md#step)
* [title](_index_d_._plugin_.inputbox.md#title)
* [totalSteps](_index_d_._plugin_.inputbox.md#totalsteps)
* [validationMessage](_index_d_._plugin_.inputbox.md#validationmessage)
* [value](_index_d_._plugin_.inputbox.md#value)

### Methods

* [dispose](_index_d_._plugin_.inputbox.md#dispose)
* [hide](_index_d_._plugin_.inputbox.md#hide)
* [show](_index_d_._plugin_.inputbox.md#show)

## Properties

### busy

•  **busy**: boolean

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[busy](_index_d_._plugin_.quickinput.md#busy)*

*Defined in [index.d.ts:9738](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9738)*

If the UI should show a progress indicator. Defaults to false.

Change this to true, e.g., while loading more data or validating
user input.

___

### buttons

•  **buttons**: ReadonlyArray\<[QuickInputButton](_index_d_._plugin_.quickinputbutton.md)>

*Defined in [index.d.ts:9896](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9896)*

Buttons for actions in the UI.

___

### enabled

•  **enabled**: boolean

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[enabled](_index_d_._plugin_.quickinput.md#enabled)*

*Defined in [index.d.ts:9730](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9730)*

If the UI should allow for user input. Defaults to true.

Change this to false, e.g., while validating user input or
loading data for the next step in user input.

___

### ignoreFocusOut

•  **ignoreFocusOut**: boolean

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[ignoreFocusOut](_index_d_._plugin_.quickinput.md#ignorefocusout)*

*Defined in [index.d.ts:9743](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9743)*

If the UI should stay open even when loosing UI focus. Defaults to false.

___

### onDidAccept

• `Readonly` **onDidAccept**: [Event](_index_d_._plugin_.event.md)\<void>

*Defined in [index.d.ts:9891](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9891)*

An event signaling when the user indicated acceptance of the input value.

___

### onDidChangeValue

• `Readonly` **onDidChangeValue**: [Event](_index_d_._plugin_.event.md)\<string>

*Defined in [index.d.ts:9886](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9886)*

An event signaling when the value has changed.

___

### onDidHide

•  **onDidHide**: [Event](_index_d_._plugin_.event.md)\<void>

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[onDidHide](_index_d_._plugin_.quickinput.md#ondidhide)*

*Defined in [index.d.ts:9765](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9765)*

An event signaling when this input UI is hidden.

There are several reasons why this UI might have to be hidden and
the extension will be notified through [QuickInput.onDidHide](#QuickInput.onDidHide).
(Examples include: an explicit call to [QuickInput.hide](#QuickInput.hide),
the user pressing Esc, some other input UI opening, etc.)

___

### onDidTriggerButton

• `Readonly` **onDidTriggerButton**: [Event](_index_d_._plugin_.event.md)\<[QuickInputButton](_index_d_._plugin_.quickinputbutton.md)>

*Defined in [index.d.ts:9901](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9901)*

An event signaling when a button was triggered.

___

### password

•  **password**: boolean

*Defined in [index.d.ts:9881](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9881)*

If the input value should be hidden. Defaults to false.

___

### placeholder

•  **placeholder**: string \| undefined

*Defined in [index.d.ts:9876](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9876)*

Optional placeholder in the filter text.

___

### prompt

•  **prompt**: string \| undefined

*Defined in [index.d.ts:9906](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9906)*

An optional prompt text providing some ask or explanation to the user.

___

### step

•  **step**: number \| undefined

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[step](_index_d_._plugin_.quickinput.md#step)*

*Defined in [index.d.ts:9717](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9717)*

An optional current step count.

___

### title

•  **title**: string \| undefined

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[title](_index_d_._plugin_.quickinput.md#title)*

*Defined in [index.d.ts:9712](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9712)*

An optional title.

___

### totalSteps

•  **totalSteps**: number \| undefined

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[totalSteps](_index_d_._plugin_.quickinput.md#totalsteps)*

*Defined in [index.d.ts:9722](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9722)*

An optional total step count.

___

### validationMessage

•  **validationMessage**: string \| undefined

*Defined in [index.d.ts:9911](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9911)*

An optional validation message indicating a problem with the current input value.

___

### value

•  **value**: string

*Defined in [index.d.ts:9871](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9871)*

Current input value.

## Methods

### dispose

▸ **dispose**(): void

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[dispose](_index_d_._plugin_.quickinput.md#dispose)*

*Defined in [index.d.ts:9773](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9773)*

Dispose of this input UI and any associated resources. If it is still
visible, it is first hidden. After this call the input UI is no longer
functional and no additional methods or properties on it should be
accessed. Instead a new input UI should be created.

**Returns:** void

___

### hide

▸ **hide**(): void

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[hide](_index_d_._plugin_.quickinput.md#hide)*

*Defined in [index.d.ts:9755](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9755)*

Hides this input UI. This will also fire an [QuickInput.onDidHide](#QuickInput.onDidHide)
event.

**Returns:** void

___

### show

▸ **show**(): void

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[show](_index_d_._plugin_.quickinput.md#show)*

*Defined in [index.d.ts:9749](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L9749)*

Makes the input UI visible in its current configuration. Any other input
UI will first fire an [QuickInput.onDidHide](#QuickInput.onDidHide) event.

**Returns:** void
