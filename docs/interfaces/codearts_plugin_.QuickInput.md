[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / QuickInput

# Interface: QuickInput

["@codearts/plugin"](../modules/_codearts_plugin_.md).QuickInput

A light-weight user input UI that is initially not visible. After
configuring it through its properties the extension can make it
visible by calling [show](codearts_plugin_.QuickInput.md#show).

There are several reasons why this UI might have to be hidden and
the extension will be notified through [onDidHide](codearts_plugin_.QuickInput.md#ondidhide).
(Examples include: an explicit call to [hide](codearts_plugin_.QuickInput.md#hide),
the user pressing Esc, some other input UI opening, etc.)

A user pressing Enter or some other gesture implying acceptance
of the current state does not automatically hide this UI component.
It is up to the extension to decide whether to accept the user's input
and if the UI should indeed be hidden through a call to [hide](codearts_plugin_.QuickInput.md#hide).

When the extension no longer needs this input UI, it should
[dispose](codearts_plugin_.QuickInput.md#dispose) it to allow for freeing up
any resources associated with it.

See [QuickPick](codearts_plugin_.QuickPick.md) and [InputBox](codearts_plugin_.InputBox.md) for concrete UIs.

## Hierarchy

- **`QuickInput`**

  ↳ [`QuickPick`](codearts_plugin_.QuickPick.md)

  ↳ [`InputBox`](codearts_plugin_.InputBox.md)

## Table of contents

### Properties

- [busy](codearts_plugin_.QuickInput.md#busy)
- [enabled](codearts_plugin_.QuickInput.md#enabled)
- [ignoreFocusOut](codearts_plugin_.QuickInput.md#ignorefocusout)
- [onDidHide](codearts_plugin_.QuickInput.md#ondidhide)
- [step](codearts_plugin_.QuickInput.md#step)
- [title](codearts_plugin_.QuickInput.md#title)
- [totalSteps](codearts_plugin_.QuickInput.md#totalsteps)

### Methods

- [dispose](codearts_plugin_.QuickInput.md#dispose)
- [hide](codearts_plugin_.QuickInput.md#hide)
- [show](codearts_plugin_.QuickInput.md#show)

## Properties

### busy

• **busy**: `boolean`

If the UI should show a progress indicator. Defaults to false.

Change this to true, e.g., while loading more data or validating
user input.

#### Defined in

[index.d.ts:11606](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11606)

___

### enabled

• **enabled**: `boolean`

If the UI should allow for user input. Defaults to true.

Change this to false, e.g., while validating user input or
loading data for the next step in user input.

#### Defined in

[index.d.ts:11598](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11598)

___

### ignoreFocusOut

• **ignoreFocusOut**: `boolean`

If the UI should stay open even when loosing UI focus. Defaults to false.
This setting is ignored on iPad and is always false.

#### Defined in

[index.d.ts:11612](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11612)

___

### onDidHide

• **onDidHide**: [`Event`](codearts_plugin_.Event.md)<`void`\>

An event signaling when this input UI is hidden.

There are several reasons why this UI might have to be hidden and
the extension will be notified through [onDidHide](codearts_plugin_.QuickInput.md#ondidhide).
(Examples include: an explicit call to [hide](codearts_plugin_.QuickInput.md#hide),
the user pressing Esc, some other input UI opening, etc.)

#### Defined in

[index.d.ts:11634](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11634)

___

### step

• **step**: `undefined` \| `number`

An optional current step count.

#### Defined in

[index.d.ts:11585](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11585)

___

### title

• **title**: `undefined` \| `string`

An optional title.

#### Defined in

[index.d.ts:11580](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11580)

___

### totalSteps

• **totalSteps**: `undefined` \| `number`

An optional total step count.

#### Defined in

[index.d.ts:11590](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11590)

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

[index.d.ts:11642](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11642)

___

### hide

▸ **hide**(): `void`

Hides this input UI. This will also fire an [onDidHide](codearts_plugin_.QuickInput.md#ondidhide)
event.

#### Returns

`void`

#### Defined in

[index.d.ts:11624](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11624)

___

### show

▸ **show**(): `void`

Makes the input UI visible in its current configuration. Any other input
UI will first fire an [onDidHide](codearts_plugin_.QuickInput.md#ondidhide) event.

#### Returns

`void`

#### Defined in

[index.d.ts:11618](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L11618)
