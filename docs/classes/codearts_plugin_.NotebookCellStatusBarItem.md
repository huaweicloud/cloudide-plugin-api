[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookCellStatusBarItem

# Class: NotebookCellStatusBarItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookCellStatusBarItem

A contribution to a cell's status bar

## Table of contents

### Constructors

- [constructor](codearts_plugin_.NotebookCellStatusBarItem.md#constructor)

### Properties

- [accessibilityInformation](codearts_plugin_.NotebookCellStatusBarItem.md#accessibilityinformation)
- [alignment](codearts_plugin_.NotebookCellStatusBarItem.md#alignment)
- [command](codearts_plugin_.NotebookCellStatusBarItem.md#command)
- [priority](codearts_plugin_.NotebookCellStatusBarItem.md#priority)
- [text](codearts_plugin_.NotebookCellStatusBarItem.md#text)
- [tooltip](codearts_plugin_.NotebookCellStatusBarItem.md#tooltip)

## Constructors

### constructor

• **new NotebookCellStatusBarItem**(`text`, `alignment`)

Creates a new NotebookCellStatusBarItem.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | The text to show for the item. |
| `alignment` | [`NotebookCellStatusBarAlignment`](../enums/codearts_plugin_.NotebookCellStatusBarAlignment.md) | Whether the item is aligned to the left or right. |

#### Defined in

[index.d.ts:14652](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14652)

## Properties

### accessibilityInformation

• `Optional` **accessibilityInformation**: [`AccessibilityInformation`](../interfaces/codearts_plugin_.AccessibilityInformation.md)

Accessibility information used when a screen reader interacts with this item.

#### Defined in

[index.d.ts:14645](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14645)

___

### alignment

• **alignment**: [`NotebookCellStatusBarAlignment`](../enums/codearts_plugin_.NotebookCellStatusBarAlignment.md)

Whether the item is aligned to the left or right.

#### Defined in

[index.d.ts:14620](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14620)

___

### command

• `Optional` **command**: `string` \| [`Command`](../interfaces/codearts_plugin_.Command.md)

An optional [`Command`](../interfaces/codearts_plugin_.Command.md) or identifier of a command to run on click.

The command must be [known](../modules/codearts_plugin_.commands.md#getcommands).

Note that if this is a [`Command`](../interfaces/codearts_plugin_.Command.md) object, only the [`command`](../interfaces/codearts_plugin_.Command.md#command) and [`arguments`](../interfaces/codearts_plugin_.Command.md#arguments)
are used by the editor.

#### Defined in

[index.d.ts:14630](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14630)

___

### priority

• `Optional` **priority**: `number`

The priority of the item. A higher value item will be shown more to the left.

#### Defined in

[index.d.ts:14640](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14640)

___

### text

• **text**: `string`

The text to show for the item.

#### Defined in

[index.d.ts:14615](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14615)

___

### tooltip

• `Optional` **tooltip**: `string`

A tooltip to show when the item is hovered.

#### Defined in

[index.d.ts:14635](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14635)
