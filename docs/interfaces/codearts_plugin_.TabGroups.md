[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TabGroups

# Interface: TabGroups

["@codearts/plugin"](../modules/_codearts_plugin_.md).TabGroups

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

#### Defined in

[index.d.ts:16098](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L16098)

___

### all

• `Readonly` **all**: readonly [`TabGroup`](codearts_plugin_.TabGroup.md)[]

#### Defined in

[index.d.ts:16093](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L16093)

___

### onDidChangeTabGroups

• `Readonly` **onDidChangeTabGroups**: [`Event`](codearts_plugin_.Event.md)<[`TabGroupChangeEvent`](codearts_plugin_.TabGroupChangeEvent.md)\>

#### Defined in

[index.d.ts:16103](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L16103)

___

### onDidChangeTabs

• `Readonly` **onDidChangeTabs**: [`Event`](codearts_plugin_.Event.md)<[`TabChangeEvent`](codearts_plugin_.TabChangeEvent.md)\>

#### Defined in

[index.d.ts:16108](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L16108)

## Methods

### close

▸ **close**(`tab`, `preserveFocus?`): [`Thenable`](Thenable.md)<`boolean`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tab` | [`Tab`](codearts_plugin_.Tab.md) \| readonly [`Tab`](codearts_plugin_.Tab.md)[] |  |
| `preserveFocus?` | `boolean` |  |

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

#### Defined in

[index.d.ts:16119](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L16119)

▸ **close**(`tabGroup`, `preserveFocus?`): [`Thenable`](Thenable.md)<`boolean`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tabGroup` | [`TabGroup`](codearts_plugin_.TabGroup.md) \| readonly [`TabGroup`](codearts_plugin_.TabGroup.md)[] |  |
| `preserveFocus?` | `boolean` |  |

#### Returns

[`Thenable`](Thenable.md)<`boolean`\>

#### Defined in

[index.d.ts:16128](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L16128)
