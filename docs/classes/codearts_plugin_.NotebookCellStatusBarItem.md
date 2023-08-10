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

[index.d.ts:14681](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14681)

## Properties

### accessibilityInformation

• `Optional` **accessibilityInformation**: [`AccessibilityInformation`](../interfaces/codearts_plugin_.AccessibilityInformation.md)

Accessibility information used when a screen reader interacts with this item.

#### Defined in

[index.d.ts:14674](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14674)

___

### alignment

• **alignment**: [`NotebookCellStatusBarAlignment`](../enums/codearts_plugin_.NotebookCellStatusBarAlignment.md)

Whether the item is aligned to the left or right.

#### Defined in

[index.d.ts:14649](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14649)

___

### command

• `Optional` **command**: `string` \| [`Command`](../interfaces/codearts_plugin_.Command.md)

An optional [`Command`](../interfaces/codearts_plugin_.Command.md) or identifier of a command to run on click.

The command must be [known](../modules/codearts_plugin_.commands.md#getcommands).

Note that if this is a [`Command`](../interfaces/codearts_plugin_.Command.md) object, only the [`command`](../interfaces/codearts_plugin_.Command.md#command) and [`arguments`](../interfaces/codearts_plugin_.Command.md#arguments)
are used by the editor.

#### Defined in

[index.d.ts:14659](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14659)

___

### priority

• `Optional` **priority**: `number`

The priority of the item. A higher value item will be shown more to the left.

#### Defined in

[index.d.ts:14669](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14669)

___

### text

• **text**: `string`

The text to show for the item.

#### Defined in

[index.d.ts:14644](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14644)

___

### tooltip

• `Optional` **tooltip**: `string`

A tooltip to show when the item is hovered.

#### Defined in

[index.d.ts:14664](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14664)
