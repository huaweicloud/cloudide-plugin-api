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

*Defined in [index.d.ts:9873](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9873)*

Active items. This can be read and updated by the extension.

___

### busy

•  **busy**: boolean

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[busy](_index_d_._plugin_.quickinput.md#busy)*

*Defined in [index.d.ts:9770](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9770)*

If the UI should show a progress indicator. Defaults to false.

Change this to true, e.g., while loading more data or validating
user input.

___

### buttons

•  **buttons**: ReadonlyArray\<[QuickInputButton](_index_d_._plugin_.quickinputbutton.md)>

*Defined in [index.d.ts:9843](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9843)*

Buttons for actions in the UI.

___

### canSelectMany

•  **canSelectMany**: boolean

*Defined in [index.d.ts:9858](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9858)*

If multiple items can be selected at the same time. Defaults to false.

___

### enabled

•  **enabled**: boolean

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[enabled](_index_d_._plugin_.quickinput.md#enabled)*

*Defined in [index.d.ts:9762](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9762)*

If the UI should allow for user input. Defaults to true.

Change this to false, e.g., while validating user input or
loading data for the next step in user input.

___

### ignoreFocusOut

•  **ignoreFocusOut**: boolean

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[ignoreFocusOut](_index_d_._plugin_.quickinput.md#ignorefocusout)*

*Defined in [index.d.ts:9775](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9775)*

If the UI should stay open even when loosing UI focus. Defaults to false.

___

### items

•  **items**: ReadonlyArray\<T>

*Defined in [index.d.ts:9853](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9853)*

Items to pick from.

___

### matchOnDescription

•  **matchOnDescription**: boolean

*Defined in [index.d.ts:9863](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9863)*

If the filter text should also be matched against the description of the items. Defaults to false.

___

### matchOnDetail

•  **matchOnDetail**: boolean

*Defined in [index.d.ts:9868](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9868)*

If the filter text should also be matched against the detail of the items. Defaults to false.

___

### onDidAccept

• `Readonly` **onDidAccept**: [Event](_index_d_._plugin_.event.md)\<void>

*Defined in [index.d.ts:9838](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9838)*

An event signaling when the user indicated acceptance of the selected item(s).

___

### onDidChangeActive

• `Readonly` **onDidChangeActive**: [Event](_index_d_._plugin_.event.md)\<T[]>

*Defined in [index.d.ts:9878](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9878)*

An event signaling when the active items have changed.

___

### onDidChangeSelection

• `Readonly` **onDidChangeSelection**: [Event](_index_d_._plugin_.event.md)\<T[]>

*Defined in [index.d.ts:9888](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9888)*

An event signaling when the selected items have changed.

___

### onDidChangeValue

• `Readonly` **onDidChangeValue**: [Event](_index_d_._plugin_.event.md)\<string>

*Defined in [index.d.ts:9833](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9833)*

An event signaling when the value of the filter text has changed.

___

### onDidHide

•  **onDidHide**: [Event](_index_d_._plugin_.event.md)\<void>

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[onDidHide](_index_d_._plugin_.quickinput.md#ondidhide)*

*Defined in [index.d.ts:9797](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9797)*

An event signaling when this input UI is hidden.

There are several reasons why this UI might have to be hidden and
the extension will be notified through [QuickInput.onDidHide](#QuickInput.onDidHide).
(Examples include: an explicit call to [QuickInput.hide](#QuickInput.hide),
the user pressing Esc, some other input UI opening, etc.)

___

### onDidTriggerButton

• `Readonly` **onDidTriggerButton**: [Event](_index_d_._plugin_.event.md)\<[QuickInputButton](_index_d_._plugin_.quickinputbutton.md)>

*Defined in [index.d.ts:9848](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9848)*

An event signaling when a button was triggered.

___

### placeholder

•  **placeholder**: string \| undefined

*Defined in [index.d.ts:9828](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9828)*

Optional placeholder in the filter text.

___

### selectedItems

•  **selectedItems**: ReadonlyArray\<T>

*Defined in [index.d.ts:9883](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9883)*

Selected items. This can be read and updated by the extension.

___

### step

•  **step**: number \| undefined

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[step](_index_d_._plugin_.quickinput.md#step)*

*Defined in [index.d.ts:9749](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9749)*

An optional current step count.

___

### title

•  **title**: string \| undefined

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[title](_index_d_._plugin_.quickinput.md#title)*

*Defined in [index.d.ts:9744](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9744)*

An optional title.

___

### totalSteps

•  **totalSteps**: number \| undefined

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[totalSteps](_index_d_._plugin_.quickinput.md#totalsteps)*

*Defined in [index.d.ts:9754](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9754)*

An optional total step count.

___

### value

•  **value**: string

*Defined in [index.d.ts:9823](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9823)*

Current value of the filter text.

## Methods

### dispose

▸ **dispose**(): void

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[dispose](_index_d_._plugin_.quickinput.md#dispose)*

*Defined in [index.d.ts:9805](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9805)*

Dispose of this input UI and any associated resources. If it is still
visible, it is first hidden. After this call the input UI is no longer
functional and no additional methods or properties on it should be
accessed. Instead a new input UI should be created.

**Returns:** void

___

### hide

▸ **hide**(): void

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[hide](_index_d_._plugin_.quickinput.md#hide)*

*Defined in [index.d.ts:9787](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9787)*

Hides this input UI. This will also fire an [QuickInput.onDidHide](#QuickInput.onDidHide)
event.

**Returns:** void

___

### show

▸ **show**(): void

*Inherited from [QuickInput](_index_d_._plugin_.quickinput.md).[show](_index_d_._plugin_.quickinput.md#show)*

*Defined in [index.d.ts:9781](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9781)*

Makes the input UI visible in its current configuration. Any other input
UI will first fire an [QuickInput.onDidHide](#QuickInput.onDidHide) event.

**Returns:** void
