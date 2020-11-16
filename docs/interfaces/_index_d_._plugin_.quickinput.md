**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / QuickInput

# Interface: QuickInput

A light-weight user input UI that is initially not visible. After
configuring it through its properties the extension can make it
visible by calling [QuickInput.show](#QuickInput.show).

There are several reasons why this UI might have to be hidden and
the extension will be notified through [QuickInput.onDidHide](#QuickInput.onDidHide).
(Examples include: an explicit call to [QuickInput.hide](#QuickInput.hide),
the user pressing Esc, some other input UI opening, etc.)

A user pressing Enter or some other gesture implying acceptance
of the current state does not automatically hide this UI component.
It is up to the extension to decide whether to accept the user's input
and if the UI should indeed be hidden through a call to [QuickInput.hide](#QuickInput.hide).

When the extension no longer needs this input UI, it should
[QuickInput.dispose](#QuickInput.dispose) it to allow for freeing up
any resources associated with it.

See [QuickPick](#QuickPick) and [InputBox](#InputBox) for concrete UIs.

## Hierarchy

* **QuickInput**

  ↳ [QuickPick](_index_d_._plugin_.quickpick.md)

  ↳ [InputBox](_index_d_._plugin_.inputbox.md)

## Index

### Properties

* [busy](_index_d_._plugin_.quickinput.md#busy)
* [enabled](_index_d_._plugin_.quickinput.md#enabled)
* [ignoreFocusOut](_index_d_._plugin_.quickinput.md#ignorefocusout)
* [onDidHide](_index_d_._plugin_.quickinput.md#ondidhide)
* [step](_index_d_._plugin_.quickinput.md#step)
* [title](_index_d_._plugin_.quickinput.md#title)
* [totalSteps](_index_d_._plugin_.quickinput.md#totalsteps)

### Methods

* [dispose](_index_d_._plugin_.quickinput.md#dispose)
* [hide](_index_d_._plugin_.quickinput.md#hide)
* [show](_index_d_._plugin_.quickinput.md#show)

## Properties

### busy

•  **busy**: boolean

*Defined in [index.d.ts:8400](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8400)*

If the UI should show a progress indicator. Defaults to false.

Change this to true, e.g., while loading more data or validating
user input.

___

### enabled

•  **enabled**: boolean

*Defined in [index.d.ts:8392](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8392)*

If the UI should allow for user input. Defaults to true.

Change this to false, e.g., while validating user input or
loading data for the next step in user input.

___

### ignoreFocusOut

•  **ignoreFocusOut**: boolean

*Defined in [index.d.ts:8405](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8405)*

If the UI should stay open even when loosing UI focus. Defaults to false.

___

### onDidHide

•  **onDidHide**: [Event](_index_d_._plugin_.event.md)\<void>

*Defined in [index.d.ts:8427](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8427)*

An event signaling when this input UI is hidden.

There are several reasons why this UI might have to be hidden and
the extension will be notified through [QuickInput.onDidHide](#QuickInput.onDidHide).
(Examples include: an explicit call to [QuickInput.hide](#QuickInput.hide),
the user pressing Esc, some other input UI opening, etc.)

___

### step

•  **step**: number \| undefined

*Defined in [index.d.ts:8379](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8379)*

An optional current step count.

___

### title

•  **title**: string \| undefined

*Defined in [index.d.ts:8374](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8374)*

An optional title.

___

### totalSteps

•  **totalSteps**: number \| undefined

*Defined in [index.d.ts:8384](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8384)*

An optional total step count.

## Methods

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:8435](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8435)*

Dispose of this input UI and any associated resources. If it is still
visible, it is first hidden. After this call the input UI is no longer
functional and no additional methods or properties on it should be
accessed. Instead a new input UI should be created.

**Returns:** void

___

### hide

▸ **hide**(): void

*Defined in [index.d.ts:8417](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8417)*

Hides this input UI. This will also fire an [QuickInput.onDidHide](#QuickInput.onDidHide)
event.

**Returns:** void

___

### show

▸ **show**(): void

*Defined in [index.d.ts:8411](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8411)*

Makes the input UI visible in its current configuration. Any other input
UI will first fire an [QuickInput.onDidHide](#QuickInput.onDidHide) event.

**Returns:** void
