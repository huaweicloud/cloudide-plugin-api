[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / QuickPick

# Interface: QuickPick<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).QuickPick

A concrete [QuickInput](codearts_plugin_.QuickInput.md) to let the user pick an item from a
list of items of type T. The items can be filtered through a filter text field and
there is an option [canSelectMany](codearts_plugin_.QuickPick.md#canselectmany) to allow for
selecting multiple items.

Note that in many cases the more convenient [showQuickPick](../modules/codearts_plugin_.window.md#showquickpick)
is easier to use. [createQuickPick](../modules/codearts_plugin_.window.md#createquickpick) should be used
when [showQuickPick](../modules/codearts_plugin_.window.md#showquickpick) does not offer the required flexibility.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`QuickPickItem`](codearts_plugin_.QuickPickItem.md) |

## Hierarchy

- [`QuickInput`](codearts_plugin_.QuickInput.md)

  ↳ **`QuickPick`**

## Table of contents

### Properties

- [activeItems](codearts_plugin_.QuickPick.md#activeitems)
- [busy](codearts_plugin_.QuickPick.md#busy)
- [buttons](codearts_plugin_.QuickPick.md#buttons)
- [canSelectMany](codearts_plugin_.QuickPick.md#canselectmany)
- [enabled](codearts_plugin_.QuickPick.md#enabled)
- [ignoreFocusOut](codearts_plugin_.QuickPick.md#ignorefocusout)
- [items](codearts_plugin_.QuickPick.md#items)
- [keepScrollPosition](codearts_plugin_.QuickPick.md#keepscrollposition)
- [matchOnDescription](codearts_plugin_.QuickPick.md#matchondescription)
- [matchOnDetail](codearts_plugin_.QuickPick.md#matchondetail)
- [onDidAccept](codearts_plugin_.QuickPick.md#ondidaccept)
- [onDidChangeActive](codearts_plugin_.QuickPick.md#ondidchangeactive)
- [onDidChangeSelection](codearts_plugin_.QuickPick.md#ondidchangeselection)
- [onDidChangeValue](codearts_plugin_.QuickPick.md#ondidchangevalue)
- [onDidHide](codearts_plugin_.QuickPick.md#ondidhide)
- [onDidTriggerButton](codearts_plugin_.QuickPick.md#ondidtriggerbutton)
- [onDidTriggerItemButton](codearts_plugin_.QuickPick.md#ondidtriggeritembutton)
- [placeholder](codearts_plugin_.QuickPick.md#placeholder)
- [selectedItems](codearts_plugin_.QuickPick.md#selecteditems)
- [step](codearts_plugin_.QuickPick.md#step)
- [title](codearts_plugin_.QuickPick.md#title)
- [totalSteps](codearts_plugin_.QuickPick.md#totalsteps)
- [value](codearts_plugin_.QuickPick.md#value)

### Methods

- [dispose](codearts_plugin_.QuickPick.md#dispose)
- [hide](codearts_plugin_.QuickPick.md#hide)
- [show](codearts_plugin_.QuickPick.md#show)

## Properties

### activeItems

• **activeItems**: readonly `T`[]

Active items. This can be read and updated by the extension.

#### Defined in

[index.d.ts:11722](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11722)

___

### busy

• **busy**: `boolean`

If the UI should show a progress indicator. Defaults to false.

Change this to true, e.g., while loading more data or validating
user input.

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[busy](codearts_plugin_.QuickInput.md#busy)

#### Defined in

[index.d.ts:11606](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11606)

___

### buttons

• **buttons**: readonly [`QuickInputButton`](codearts_plugin_.QuickInputButton.md)[]

Buttons for actions in the UI.

#### Defined in

[index.d.ts:11680](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11680)

___

### canSelectMany

• **canSelectMany**: `boolean`

If multiple items can be selected at the same time. Defaults to false.

#### Defined in

[index.d.ts:11702](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11702)

___

### enabled

• **enabled**: `boolean`

If the UI should allow for user input. Defaults to true.

Change this to false, e.g., while validating user input or
loading data for the next step in user input.

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[enabled](codearts_plugin_.QuickInput.md#enabled)

#### Defined in

[index.d.ts:11598](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11598)

___

### ignoreFocusOut

• **ignoreFocusOut**: `boolean`

If the UI should stay open even when loosing UI focus. Defaults to false.
This setting is ignored on iPad and is always false.

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[ignoreFocusOut](codearts_plugin_.QuickInput.md#ignorefocusout)

#### Defined in

[index.d.ts:11612](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11612)

___

### items

• **items**: readonly `T`[]

Items to pick from. This can be read and updated by the extension.

#### Defined in

[index.d.ts:11697](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11697)

___

### keepScrollPosition

• `Optional` **keepScrollPosition**: `boolean`

#### Defined in

[index.d.ts:11717](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11717)

___

### matchOnDescription

• **matchOnDescription**: `boolean`

If the filter text should also be matched against the description of the items. Defaults to false.

#### Defined in

[index.d.ts:11707](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11707)

___

### matchOnDetail

• **matchOnDetail**: `boolean`

If the filter text should also be matched against the detail of the items. Defaults to false.

#### Defined in

[index.d.ts:11712](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11712)

___

### onDidAccept

• `Readonly` **onDidAccept**: [`Event`](codearts_plugin_.Event.md)<`void`\>

An event signaling when the user indicated acceptance of the selected item(s).

#### Defined in

[index.d.ts:11675](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11675)

___

### onDidChangeActive

• `Readonly` **onDidChangeActive**: [`Event`](codearts_plugin_.Event.md)<readonly `T`[]\>

An event signaling when the active items have changed.

#### Defined in

[index.d.ts:11727](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11727)

___

### onDidChangeSelection

• `Readonly` **onDidChangeSelection**: [`Event`](codearts_plugin_.Event.md)<readonly `T`[]\>

An event signaling when the selected items have changed.

#### Defined in

[index.d.ts:11737](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11737)

___

### onDidChangeValue

• `Readonly` **onDidChangeValue**: [`Event`](codearts_plugin_.Event.md)<`string`\>

An event signaling when the value of the filter text has changed.

#### Defined in

[index.d.ts:11670](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11670)

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

[index.d.ts:11634](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11634)

___

### onDidTriggerButton

• `Readonly` **onDidTriggerButton**: [`Event`](codearts_plugin_.Event.md)<[`QuickInputButton`](codearts_plugin_.QuickInputButton.md)\>

An event signaling when a button in the title bar was triggered.
This event does not fire for buttons on a [QuickPickItem](codearts_plugin_.QuickPickItem.md).

#### Defined in

[index.d.ts:11686](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11686)

___

### onDidTriggerItemButton

• `Readonly` **onDidTriggerItemButton**: [`Event`](codearts_plugin_.Event.md)<[`QuickPickItemButtonEvent`](codearts_plugin_.QuickPickItemButtonEvent.md)<`T`\>\>

An event signaling when a button in a particular [QuickPickItem](codearts_plugin_.QuickPickItem.md) was triggered.
This event does not fire for buttons in the title bar.

#### Defined in

[index.d.ts:11692](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11692)

___

### placeholder

• **placeholder**: `undefined` \| `string`

Optional placeholder in the filter text.

#### Defined in

[index.d.ts:11665](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11665)

___

### selectedItems

• **selectedItems**: readonly `T`[]

Selected items. This can be read and updated by the extension.

#### Defined in

[index.d.ts:11732](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11732)

___

### step

• **step**: `undefined` \| `number`

An optional current step count.

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[step](codearts_plugin_.QuickInput.md#step)

#### Defined in

[index.d.ts:11585](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11585)

___

### title

• **title**: `undefined` \| `string`

An optional title.

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[title](codearts_plugin_.QuickInput.md#title)

#### Defined in

[index.d.ts:11580](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11580)

___

### totalSteps

• **totalSteps**: `undefined` \| `number`

An optional total step count.

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[totalSteps](codearts_plugin_.QuickInput.md#totalsteps)

#### Defined in

[index.d.ts:11590](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11590)

___

### value

• **value**: `string`

Current value of the filter text.

#### Defined in

[index.d.ts:11660](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11660)

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

[index.d.ts:11642](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11642)

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

[index.d.ts:11624](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11624)

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

[index.d.ts:11618](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11618)
