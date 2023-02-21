[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / StatusBarItem

# Interface: StatusBarItem

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).StatusBarItem

A status bar item is a status bar contribution that can
show text and icons and run a command on click.

## Table of contents

### Properties

- [alignment](cloudide_plugin_.StatusBarItem.md#alignment)
- [color](cloudide_plugin_.StatusBarItem.md#color)
- [command](cloudide_plugin_.StatusBarItem.md#command)
- [priority](cloudide_plugin_.StatusBarItem.md#priority)
- [text](cloudide_plugin_.StatusBarItem.md#text)
- [tooltip](cloudide_plugin_.StatusBarItem.md#tooltip)

### Methods

- [dispose](cloudide_plugin_.StatusBarItem.md#dispose)
- [hide](cloudide_plugin_.StatusBarItem.md#hide)
- [show](cloudide_plugin_.StatusBarItem.md#show)

## Properties

### alignment

• `Readonly` **alignment**: [`StatusBarAlignment`](../enums/cloudide_plugin_.StatusBarAlignment.md)

The alignment of this item.

#### Defined in

[index.d.ts:2508](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2508)

___

### color

• **color**: `undefined` \| `string` \| [`ThemeColor`](../classes/cloudide_plugin_.ThemeColor.md)

The foreground color for this entry.

#### Defined in

[index.d.ts:2530](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2530)

___

### command

• **command**: `undefined` \| `string` \| [`Command`](cloudide_plugin_.Command.md)

The identifier of a command to run on click.

#### Defined in

[index.d.ts:2535](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2535)

___

### priority

• `Readonly` **priority**: `number`

The priority of this item. Higher value means the item should
be shown more to the left.

#### Defined in

[index.d.ts:2514](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2514)

___

### text

• **text**: `string`

The text to show for the entry. To set a text with icon use the following pattern in text string:
$(fontawesomeClassName)

#### Defined in

[index.d.ts:2520](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2520)

___

### tooltip

• **tooltip**: `undefined` \| `string`

The tooltip text when you hover over this entry.

#### Defined in

[index.d.ts:2525](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2525)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose and free associated resources. Hide the entry in the status bar.

#### Returns

`void`

#### Defined in

[index.d.ts:2550](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2550)

___

### hide

▸ **hide**(): `void`

Hide the entry in the status bar.

#### Returns

`void`

#### Defined in

[index.d.ts:2545](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2545)

___

### show

▸ **show**(): `void`

Shows the entry in the status bar.

#### Returns

`void`

#### Defined in

[index.d.ts:2540](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2540)
