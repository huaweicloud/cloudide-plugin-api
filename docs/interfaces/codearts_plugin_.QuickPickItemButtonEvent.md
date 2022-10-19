[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / QuickPickItemButtonEvent

# Interface: QuickPickItemButtonEvent<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).QuickPickItemButtonEvent

An event signaling when a button in a particular [QuickPickItem](codearts_plugin_.QuickPickItem.md) was triggered.
This event does not fire for buttons in the title bar.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`QuickPickItem`](codearts_plugin_.QuickPickItem.md) |

## Table of contents

### Properties

- [button](codearts_plugin_.QuickPickItemButtonEvent.md#button)
- [item](codearts_plugin_.QuickPickItemButtonEvent.md#item)

## Properties

### button

• `Readonly` **button**: [`QuickInputButton`](codearts_plugin_.QuickInputButton.md)

The button that was clicked.

#### Defined in

[index.d.ts:11430](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L11430)

___

### item

• `Readonly` **item**: `T`

The item that the button belongs to.

#### Defined in

[index.d.ts:11434](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L11434)
