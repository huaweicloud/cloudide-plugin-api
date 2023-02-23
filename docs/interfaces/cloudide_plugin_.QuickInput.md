[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / QuickInput

# Interface: QuickInput

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).QuickInput

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

- **`QuickInput`**

  ↳ [`QuickPick`](cloudide_plugin_.QuickPick.md)

  ↳ [`InputBox`](cloudide_plugin_.InputBox.md)

## Table of contents

### Properties

- [busy](cloudide_plugin_.QuickInput.md#busy)
- [enabled](cloudide_plugin_.QuickInput.md#enabled)
- [ignoreFocusOut](cloudide_plugin_.QuickInput.md#ignorefocusout)
- [onDidHide](cloudide_plugin_.QuickInput.md#ondidhide)
- [step](cloudide_plugin_.QuickInput.md#step)
- [title](cloudide_plugin_.QuickInput.md#title)
- [totalSteps](cloudide_plugin_.QuickInput.md#totalsteps)

### Methods

- [dispose](cloudide_plugin_.QuickInput.md#dispose)
- [hide](cloudide_plugin_.QuickInput.md#hide)
- [show](cloudide_plugin_.QuickInput.md#show)

## Properties

### busy

• **busy**: `boolean`

If the UI should show a progress indicator. Defaults to false.

Change this to true, e.g., while loading more data or validating
user input.

#### Defined in

[index.d.ts:5046](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5046)

___

### enabled

• **enabled**: `boolean`

If the UI should allow for user input. Defaults to true.

Change this to false, e.g., while validating user input or
loading data for the next step in user input.

#### Defined in

[index.d.ts:5038](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5038)

___

### ignoreFocusOut

• **ignoreFocusOut**: `boolean`

If the UI should stay open even when loosing UI focus. Defaults to false.

#### Defined in

[index.d.ts:5051](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5051)

___

### onDidHide

• **onDidHide**: [`Event`](cloudide_plugin_.Event.md)<`void`\>

An event signaling when this input UI is hidden.

There are several reasons why this UI might have to be hidden and
the extension will be notified through [QuickInput.onDidHide](#QuickInput.onDidHide).
(Examples include: an explicit call to [QuickInput.hide](#QuickInput.hide),
the user pressing Esc, some other input UI opening, etc.)

#### Defined in

[index.d.ts:5073](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5073)

___

### step

• **step**: `undefined` \| `number`

An optional current step count.

#### Defined in

[index.d.ts:5025](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5025)

___

### title

• **title**: `undefined` \| `string`

An optional title.

#### Defined in

[index.d.ts:5020](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5020)

___

### totalSteps

• **totalSteps**: `undefined` \| `number`

An optional total step count.

#### Defined in

[index.d.ts:5030](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5030)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose of this input UI and any associated resources. If it is still
visible, it is first hidden. After this call the input UI is no longer
functional and no additional methods or properties on it should be
accessed. Instead a new input UI should be created.

#### Returns

`void`

#### Defined in

[index.d.ts:5081](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5081)

___

### hide

▸ **hide**(): `void`

Hides this input UI. This will also fire an [QuickInput.onDidHide](#QuickInput.onDidHide)
event.

#### Returns

`void`

#### Defined in

[index.d.ts:5063](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5063)

___

### show

▸ **show**(): `void`

Makes the input UI visible in its current configuration. Any other input
UI will first fire an [QuickInput.onDidHide](#QuickInput.onDidHide) event.

#### Returns

`void`

#### Defined in

[index.d.ts:5057](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5057)