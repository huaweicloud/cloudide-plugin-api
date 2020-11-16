**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / QuickPick

# Interface: QuickPick\<T>

A concrete [QuickInput](#QuickInput) to let the user pick an item from a
list of items of type T. The items can be filtered through a filter text field and
there is an option [canSelectMany](#QuickPick.canSelectMany) to allow for
selecting multiple items.

Note that in many cases the more convenient [window.showQuickPick](#window.showQuickPick)
is easier to use. [window.createQuickPick](#window.createQuickPick) should be used
when [window.showQuickPick](#window.showQuickPick) does not offer the required flexibility.

## Type parameters

Name | Type |
------ | ------ |
`T` | [QuickPickItem](_index_d_._plugin_.quickpickitem.md) |

## Hierarchy

* [QuickInput](_index_d_._plugin_.quickinput.md)

  ↳ **QuickPick**

## Index

### Properties

* [activeItems](_index_d_._plugin_.quickpick.md#activeitems)
* [busy](_index_d_._plugin_.quickpick.md#busy)
* [buttons](_index_d_._plugin_.quickpick.md#buttons)
* [canSelectMany](_index_d_._plugin_.quickpick.md#canselectmany)
* [enabled](_index_d_._plugin_.quickpick.md#enabled)
* [ignoreFocusOut](_index_d_._plugin_.quickpick.md#ignorefocusout)
* [items](_index_d_._plugin_.quickpick.md#items)
* [matchOnDescription](_index_d_._plugin_.quickpick.md#matchondescription)
* [matchOnDetail](_index_d_._plugin_.quickpick.md#matchondetail)
* [onDidAccept](_index_d_._plugin_.quickpick.md#ondidaccept)
* [onDidChangeActive](_index_d_._plugin_.quickpick.md#ondidchangeactive)
* [onDidChangeSelection](_index_d_._plugin_.quickpick.md#ondidchangeselection)
* [onDidChangeValue](_index_d_._plugin_.quickpick.md#ondidchangevalue)
* [onDidHide](_index_d_._plugin_.quickpick.md#ondidhide)
* [onDidTriggerButton](_index_d_._plugin_.quickpick.md#ondidtriggerbutton)
* [placeholder](_index_d_._plugin_.quickpick.md#placeholder)
* [selectedItems](_index_d_._plugin_.quickpick.md#selecteditems)
* [step](_index_d_._plugin_.quickpick.md#step)
* [title](_index_d_._plugin_.quickpick.md#title)
* [totalSteps](_index_d_._plugin_.quickpick.md#totalsteps)
* [value](_index_d_._plugin_.quickpick.md#value)

### Methods

* [dispose](_index_d_._plugin_.quickpick.md#dispose)
* [hide](_index_d_._plugin_.quickpick.md#hide)
* [show](_index_d_._plugin_.quickpick.md#show)

## Properties

### activeItems

•  **activeItems**: ReadonlyArray\<T>

*Defined in [index.d.ts:8503](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8503)*

Active items. This can be read and updated by the extension.

___

### busy

•  **busy**: boolean

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[busy](_index_d_._plugin_.quickinput.md#busy)*

*Defined in [index.d.ts:8400](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8400)*

If the UI should show a progress indicator. Defaults to false.

Change this to true, e.g., while loading more data or validating
user input.

___

### buttons

•  **buttons**: ReadonlyArray\<[QuickInputButton](_index_d_._plugin_.quickinputbutton.md)>

*Defined in [index.d.ts:8473](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8473)*

Buttons for actions in the UI.

___

### canSelectMany

•  **canSelectMany**: boolean

*Defined in [index.d.ts:8488](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8488)*

If multiple items can be selected at the same time. Defaults to false.

___

### enabled

•  **enabled**: boolean

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[enabled](_index_d_._plugin_.quickinput.md#enabled)*

*Defined in [index.d.ts:8392](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8392)*

If the UI should allow for user input. Defaults to true.

Change this to false, e.g., while validating user input or
loading data for the next step in user input.

___

### ignoreFocusOut

•  **ignoreFocusOut**: boolean

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[ignoreFocusOut](_index_d_._plugin_.quickinput.md#ignorefocusout)*

*Defined in [index.d.ts:8405](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8405)*

If the UI should stay open even when loosing UI focus. Defaults to false.

___

### items

•  **items**: ReadonlyArray\<T>

*Defined in [index.d.ts:8483](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8483)*

Items to pick from.

___

### matchOnDescription

•  **matchOnDescription**: boolean

*Defined in [index.d.ts:8493](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8493)*

If the filter text should also be matched against the description of the items. Defaults to false.

___

### matchOnDetail

•  **matchOnDetail**: boolean

*Defined in [index.d.ts:8498](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8498)*

If the filter text should also be matched against the detail of the items. Defaults to false.

___

### onDidAccept

• `Readonly` **onDidAccept**: [Event](_index_d_._plugin_.event.md)\<void>

*Defined in [index.d.ts:8468](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8468)*

An event signaling when the user indicated acceptance of the selected item(s).

___

### onDidChangeActive

• `Readonly` **onDidChangeActive**: [Event](_index_d_._plugin_.event.md)\<T[]>

*Defined in [index.d.ts:8508](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8508)*

An event signaling when the active items have changed.

___

### onDidChangeSelection

• `Readonly` **onDidChangeSelection**: [Event](_index_d_._plugin_.event.md)\<T[]>

*Defined in [index.d.ts:8518](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8518)*

An event signaling when the selected items have changed.

___

### onDidChangeValue

• `Readonly` **onDidChangeValue**: [Event](_index_d_._plugin_.event.md)\<string>

*Defined in [index.d.ts:8463](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8463)*

An event signaling when the value of the filter text has changed.

___

### onDidHide

•  **onDidHide**: [Event](_index_d_._plugin_.event.md)\<void>

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[onDidHide](_index_d_._plugin_.quickinput.md#ondidhide)*

*Defined in [index.d.ts:8427](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8427)*

An event signaling when this input UI is hidden.

There are several reasons why this UI might have to be hidden and
the extension will be notified through [QuickInput.onDidHide](#QuickInput.onDidHide).
(Examples include: an explicit call to [QuickInput.hide](#QuickInput.hide),
the user pressing Esc, some other input UI opening, etc.)

___

### onDidTriggerButton

• `Readonly` **onDidTriggerButton**: [Event](_index_d_._plugin_.event.md)\<[QuickInputButton](_index_d_._plugin_.quickinputbutton.md)>

*Defined in [index.d.ts:8478](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8478)*

An event signaling when a button was triggered.

___

### placeholder

•  **placeholder**: string \| undefined

*Defined in [index.d.ts:8458](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8458)*

Optional placeholder in the filter text.

___

### selectedItems

•  **selectedItems**: ReadonlyArray\<T>

*Defined in [index.d.ts:8513](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8513)*

Selected items. This can be read and updated by the extension.

___

### step

•  **step**: number \| undefined

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[step](_index_d_._plugin_.quickinput.md#step)*

*Defined in [index.d.ts:8379](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8379)*

An optional current step count.

___

### title

•  **title**: string \| undefined

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[title](_index_d_._plugin_.quickinput.md#title)*

*Defined in [index.d.ts:8374](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8374)*

An optional title.

___

### totalSteps

•  **totalSteps**: number \| undefined

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[totalSteps](_index_d_._plugin_.quickinput.md#totalsteps)*

*Defined in [index.d.ts:8384](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8384)*

An optional total step count.

___

### value

•  **value**: string

*Defined in [index.d.ts:8453](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8453)*

Current value of the filter text.

## Methods

### dispose

▸ **dispose**(): void

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[dispose](_index_d_._plugin_.quickinput.md#dispose)*

*Defined in [index.d.ts:8435](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8435)*

Dispose of this input UI and any associated resources. If it is still
visible, it is first hidden. After this call the input UI is no longer
functional and no additional methods or properties on it should be
accessed. Instead a new input UI should be created.

**Returns:** void

___

### hide

▸ **hide**(): void

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[hide](_index_d_._plugin_.quickinput.md#hide)*

*Defined in [index.d.ts:8417](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8417)*

Hides this input UI. This will also fire an [QuickInput.onDidHide](#QuickInput.onDidHide)
event.

**Returns:** void

___

### show

▸ **show**(): void

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[show](_index_d_._plugin_.quickinput.md#show)*

*Defined in [index.d.ts:8411](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8411)*

Makes the input UI visible in its current configuration. Any other input
UI will first fire an [QuickInput.onDidHide](#QuickInput.onDidHide) event.

**Returns:** void
