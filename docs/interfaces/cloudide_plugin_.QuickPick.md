[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / QuickPick

# Interface: QuickPick<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).QuickPick

A concrete [QuickInput](#QuickInput) to let the user pick an item from a
list of items of type T. The items can be filtered through a filter text field and
there is an option [canSelectMany](#QuickPick.canSelectMany) to allow for
selecting multiple items.

Note that in many cases the more convenient [window.showQuickPick](#window.showQuickPick)
is easier to use. [window.createQuickPick](#window.createQuickPick) should be used
when [window.showQuickPick](#window.showQuickPick) does not offer the required flexibility.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`QuickPickItem`](cloudide_plugin_.QuickPickItem.md) |

## Hierarchy

- [`QuickInput`](cloudide_plugin_.QuickInput.md)

  ↳ **`QuickPick`**

## Table of contents

### Properties

- [activeItems](cloudide_plugin_.QuickPick.md#activeitems)
- [busy](cloudide_plugin_.QuickPick.md#busy)
- [buttons](cloudide_plugin_.QuickPick.md#buttons)
- [canSelectMany](cloudide_plugin_.QuickPick.md#canselectmany)
- [enabled](cloudide_plugin_.QuickPick.md#enabled)
- [ignoreFocusOut](cloudide_plugin_.QuickPick.md#ignorefocusout)
- [items](cloudide_plugin_.QuickPick.md#items)
- [matchOnDescription](cloudide_plugin_.QuickPick.md#matchondescription)
- [matchOnDetail](cloudide_plugin_.QuickPick.md#matchondetail)
- [onDidAccept](cloudide_plugin_.QuickPick.md#ondidaccept)
- [onDidChangeActive](cloudide_plugin_.QuickPick.md#ondidchangeactive)
- [onDidChangeSelection](cloudide_plugin_.QuickPick.md#ondidchangeselection)
- [onDidChangeValue](cloudide_plugin_.QuickPick.md#ondidchangevalue)
- [onDidHide](cloudide_plugin_.QuickPick.md#ondidhide)
- [onDidTriggerButton](cloudide_plugin_.QuickPick.md#ondidtriggerbutton)
- [placeholder](cloudide_plugin_.QuickPick.md#placeholder)
- [selectedItems](cloudide_plugin_.QuickPick.md#selecteditems)
- [step](cloudide_plugin_.QuickPick.md#step)
- [title](cloudide_plugin_.QuickPick.md#title)
- [totalSteps](cloudide_plugin_.QuickPick.md#totalsteps)
- [value](cloudide_plugin_.QuickPick.md#value)

### Methods

- [dispose](cloudide_plugin_.QuickPick.md#dispose)
- [hide](cloudide_plugin_.QuickPick.md#hide)
- [show](cloudide_plugin_.QuickPick.md#show)

## Properties

### activeItems

• **activeItems**: readonly `T`[]

Active items. This can be read and updated by the extension.

#### Defined in

[index.d.ts:2246](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2246)

___

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

[index.d.ts:2216](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2216)

___

### canSelectMany

• **canSelectMany**: `boolean`

If multiple items can be selected at the same time. Defaults to false.

#### Defined in

[index.d.ts:2231](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2231)

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

### items

• **items**: readonly `T`[]

Items to pick from.

#### Defined in

[index.d.ts:2226](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2226)

___

### matchOnDescription

• **matchOnDescription**: `boolean`

If the filter text should also be matched against the description of the items. Defaults to false.

#### Defined in

[index.d.ts:2236](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2236)

___

### matchOnDetail

• **matchOnDetail**: `boolean`

If the filter text should also be matched against the detail of the items. Defaults to false.

#### Defined in

[index.d.ts:2241](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2241)

___

### onDidAccept

• `Readonly` **onDidAccept**: [`Event`](cloudide_plugin_.Event.md)<`void`\>

An event signaling when the user indicated acceptance of the selected item(s).

#### Defined in

[index.d.ts:2211](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2211)

___

### onDidChangeActive

• `Readonly` **onDidChangeActive**: [`Event`](cloudide_plugin_.Event.md)<`T`[]\>

An event signaling when the active items have changed.

#### Defined in

[index.d.ts:2251](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2251)

___

### onDidChangeSelection

• `Readonly` **onDidChangeSelection**: [`Event`](cloudide_plugin_.Event.md)<`T`[]\>

An event signaling when the selected items have changed.

#### Defined in

[index.d.ts:2261](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2261)

___

### onDidChangeValue

• `Readonly` **onDidChangeValue**: [`Event`](cloudide_plugin_.Event.md)<`string`\>

An event signaling when the value of the filter text has changed.

#### Defined in

[index.d.ts:2206](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2206)

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

[index.d.ts:2221](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2221)

___

### placeholder

• **placeholder**: `undefined` \| `string`

Optional placeholder in the filter text.

#### Defined in

[index.d.ts:2201](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2201)

___

### selectedItems

• **selectedItems**: readonly `T`[]

Selected items. This can be read and updated by the extension.

#### Defined in

[index.d.ts:2256](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2256)

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

### value

• **value**: `string`

Current value of the filter text.

#### Defined in

[index.d.ts:2196](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2196)

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
