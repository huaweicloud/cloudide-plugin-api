[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / QuickPick

# Interface: QuickPick<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).QuickPick

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

#### Defined in

[index.d.ts:11067](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11067)

___

### busy

• **busy**: `boolean`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[busy](codearts_plugin_.QuickInput.md#busy)

#### Defined in

[index.d.ts:10951](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10951)

___

### buttons

• **buttons**: readonly [`QuickInputButton`](codearts_plugin_.QuickInputButton.md)[]

#### Defined in

[index.d.ts:11025](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11025)

___

### canSelectMany

• **canSelectMany**: `boolean`

#### Defined in

[index.d.ts:11047](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11047)

___

### enabled

• **enabled**: `boolean`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[enabled](codearts_plugin_.QuickInput.md#enabled)

#### Defined in

[index.d.ts:10943](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10943)

___

### ignoreFocusOut

• **ignoreFocusOut**: `boolean`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[ignoreFocusOut](codearts_plugin_.QuickInput.md#ignorefocusout)

#### Defined in

[index.d.ts:10957](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10957)

___

### items

• **items**: readonly `T`[]

#### Defined in

[index.d.ts:11042](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11042)

___

### keepScrollPosition

• `Optional` **keepScrollPosition**: `boolean`

#### Defined in

[index.d.ts:11062](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11062)

___

### matchOnDescription

• **matchOnDescription**: `boolean`

#### Defined in

[index.d.ts:11052](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11052)

___

### matchOnDetail

• **matchOnDetail**: `boolean`

#### Defined in

[index.d.ts:11057](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11057)

___

### onDidAccept

• `Readonly` **onDidAccept**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Defined in

[index.d.ts:11020](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11020)

___

### onDidChangeActive

• `Readonly` **onDidChangeActive**: [`Event`](codearts_plugin_.Event.md)<readonly `T`[]\>

#### Defined in

[index.d.ts:11072](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11072)

___

### onDidChangeSelection

• `Readonly` **onDidChangeSelection**: [`Event`](codearts_plugin_.Event.md)<readonly `T`[]\>

#### Defined in

[index.d.ts:11082](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11082)

___

### onDidChangeValue

• `Readonly` **onDidChangeValue**: [`Event`](codearts_plugin_.Event.md)<`string`\>

#### Defined in

[index.d.ts:11015](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11015)

___

### onDidHide

• **onDidHide**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[onDidHide](codearts_plugin_.QuickInput.md#ondidhide)

#### Defined in

[index.d.ts:10979](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10979)

___

### onDidTriggerButton

• `Readonly` **onDidTriggerButton**: [`Event`](codearts_plugin_.Event.md)<[`QuickInputButton`](codearts_plugin_.QuickInputButton.md)\>

#### Defined in

[index.d.ts:11031](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11031)

___

### onDidTriggerItemButton

• `Readonly` **onDidTriggerItemButton**: [`Event`](codearts_plugin_.Event.md)<[`QuickPickItemButtonEvent`](codearts_plugin_.QuickPickItemButtonEvent.md)<`T`\>\>

#### Defined in

[index.d.ts:11037](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11037)

___

### placeholder

• **placeholder**: `undefined` \| `string`

#### Defined in

[index.d.ts:11010](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11010)

___

### selectedItems

• **selectedItems**: readonly `T`[]

#### Defined in

[index.d.ts:11077](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11077)

___

### step

• **step**: `undefined` \| `number`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[step](codearts_plugin_.QuickInput.md#step)

#### Defined in

[index.d.ts:10930](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10930)

___

### title

• **title**: `undefined` \| `string`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[title](codearts_plugin_.QuickInput.md#title)

#### Defined in

[index.d.ts:10925](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10925)

___

### totalSteps

• **totalSteps**: `undefined` \| `number`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[totalSteps](codearts_plugin_.QuickInput.md#totalsteps)

#### Defined in

[index.d.ts:10935](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10935)

___

### value

• **value**: `string`

#### Defined in

[index.d.ts:11005](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L11005)

## Methods

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[dispose](codearts_plugin_.QuickInput.md#dispose)

#### Defined in

[index.d.ts:10987](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10987)

___

### hide

▸ **hide**(): `void`

#### Returns

`void`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[hide](codearts_plugin_.QuickInput.md#hide)

#### Defined in

[index.d.ts:10969](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10969)

___

### show

▸ **show**(): `void`

#### Returns

`void`

#### Inherited from

[QuickInput](codearts_plugin_.QuickInput.md).[show](codearts_plugin_.QuickInput.md#show)

#### Defined in

[index.d.ts:10963](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L10963)
