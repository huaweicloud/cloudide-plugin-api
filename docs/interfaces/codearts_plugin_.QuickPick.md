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

[index.d.ts:11159](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11159)

___

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

[index.d.ts:11117](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11117)

___

### canSelectMany

• **canSelectMany**: `boolean`

If multiple items can be selected at the same time. Defaults to false.

#### Defined in

[index.d.ts:11139](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11139)

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

### items

• **items**: readonly `T`[]

Items to pick from. This can be read and updated by the extension.

#### Defined in

[index.d.ts:11134](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11134)

___

### keepScrollPosition

• `Optional` **keepScrollPosition**: `boolean`

#### Defined in

[index.d.ts:11154](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11154)

___

### matchOnDescription

• **matchOnDescription**: `boolean`

If the filter text should also be matched against the description of the items. Defaults to false.

#### Defined in

[index.d.ts:11144](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11144)

___

### matchOnDetail

• **matchOnDetail**: `boolean`

If the filter text should also be matched against the detail of the items. Defaults to false.

#### Defined in

[index.d.ts:11149](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11149)

___

### onDidAccept

• `Readonly` **onDidAccept**: [`Event`](codearts_plugin_.Event.md)<`void`\>

An event signaling when the user indicated acceptance of the selected item(s).

#### Defined in

[index.d.ts:11112](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11112)

___

### onDidChangeActive

• `Readonly` **onDidChangeActive**: [`Event`](codearts_plugin_.Event.md)<readonly `T`[]\>

An event signaling when the active items have changed.

#### Defined in

[index.d.ts:11164](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11164)

___

### onDidChangeSelection

• `Readonly` **onDidChangeSelection**: [`Event`](codearts_plugin_.Event.md)<readonly `T`[]\>

An event signaling when the selected items have changed.

#### Defined in

[index.d.ts:11174](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11174)

___

### onDidChangeValue

• `Readonly` **onDidChangeValue**: [`Event`](codearts_plugin_.Event.md)<`string`\>

An event signaling when the value of the filter text has changed.

#### Defined in

[index.d.ts:11107](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11107)

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

An event signaling when a button in the title bar was triggered.
This event does not fire for buttons on a [QuickPickItem](codearts_plugin_.QuickPickItem.md).

#### Defined in

[index.d.ts:11123](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11123)

___

### onDidTriggerItemButton

• `Readonly` **onDidTriggerItemButton**: [`Event`](codearts_plugin_.Event.md)<[`QuickPickItemButtonEvent`](codearts_plugin_.QuickPickItemButtonEvent.md)<`T`\>\>

An event signaling when a button in a particular [QuickPickItem](codearts_plugin_.QuickPickItem.md) was triggered.
This event does not fire for buttons in the title bar.

#### Defined in

[index.d.ts:11129](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11129)

___

### placeholder

• **placeholder**: `undefined` \| `string`

Optional placeholder in the filter text.

#### Defined in

[index.d.ts:11102](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11102)

___

### selectedItems

• **selectedItems**: readonly `T`[]

Selected items. This can be read and updated by the extension.

#### Defined in

[index.d.ts:11169](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11169)

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

### value

• **value**: `string`

Current value of the filter text.

#### Defined in

[index.d.ts:11097](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L11097)

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
