[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TabGroups

# Interface: TabGroups

["@codearts/plugin"](../modules/_codearts_plugin_.md).TabGroups

Represents the main editor area which consists of multple groups which contain tabs.

## Table of contents

### Properties

- [activeTabGroup](codearts_plugin_.TabGroups.md#activetabgroup)
- [all](codearts_plugin_.TabGroups.md#all)
- [onDidChangeTabGroups](codearts_plugin_.TabGroups.md#ondidchangetabgroups)
- [onDidChangeTabs](codearts_plugin_.TabGroups.md#ondidchangetabs)

### Methods

- [close](codearts_plugin_.TabGroups.md#close)

## Properties

### activeTabGroup

• `Readonly` **activeTabGroup**: [`TabGroup`](codearts_plugin_.TabGroup.md)

The currently active group.

#### Defined in

[index.d.ts:16539](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16539)

___

### all

• `Readonly` **all**: readonly [`TabGroup`](codearts_plugin_.TabGroup.md)[]

All the groups within the group container.

#### Defined in

[index.d.ts:16534](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16534)

___

### onDidChangeTabGroups

• `Readonly` **onDidChangeTabGroups**: [`Event`](codearts_plugin_.Event.md)<[`TabGroupChangeEvent`](codearts_plugin_.TabGroupChangeEvent.md)\>

An [event](codearts_plugin_.Event.md) which fires when [tab groups](codearts_plugin_.TabGroup.md) have changed.

#### Defined in

[index.d.ts:16544](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16544)

___

### onDidChangeTabs

• `Readonly` **onDidChangeTabs**: [`Event`](codearts_plugin_.Event.md)<[`TabChangeEvent`](codearts_plugin_.TabChangeEvent.md)\>

An [event](codearts_plugin_.Event.md) which fires when [tabs](codearts_plugin_.Tab.md) have changed.

#### Defined in

[index.d.ts:16549](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16549)

## Methods

### close

▸ **close**(`tab`, `preserveFocus?`): [`Thenable`](Thenable.md)<`boolean`\>

Closes the tab. This makes the tab object invalid and the tab
should no longer be used for further actions.
Note: In the case of a dirty tab, a confirmation dialog will be shown which may be cancelled. If cancelled the tab is still valid

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tab` | [`Tab`](codearts_plugin_.Tab.md) \| readonly [`Tab`](codearts_plugin_.Tab.md)[] | The tab to close. |
| `preserveFocus?` | `boolean` | When `true` focus will remain in its current position. If `false` it will jump to the next tab. |

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

A promise that resolves to `true` when all tabs have been closed.

#### Defined in

[index.d.ts:16560](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16560)

▸ **close**(`tabGroup`, `preserveFocus?`): [`Thenable`](Thenable.md)<`boolean`\>

Closes the tab group. This makes the tab group object invalid and the tab group
should no longer be used for further actions.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tabGroup` | [`TabGroup`](codearts_plugin_.TabGroup.md) \| readonly [`TabGroup`](codearts_plugin_.TabGroup.md)[] | The tab group to close. |
| `preserveFocus?` | `boolean` | When `true` focus will remain in its current position. |

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

A promise that resolves to `true` when all tab groups have been closed.

#### Defined in

[index.d.ts:16569](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16569)
