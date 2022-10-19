[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / StatusBarItem

# Interface: StatusBarItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).StatusBarItem

A status bar item is a status bar contribution that can
show text and icons and run a command on click.

## Table of contents

### Properties

- [accessibilityInformation](codearts_plugin_.StatusBarItem.md#accessibilityinformation)
- [alignment](codearts_plugin_.StatusBarItem.md#alignment)
- [backgroundColor](codearts_plugin_.StatusBarItem.md#backgroundcolor)
- [color](codearts_plugin_.StatusBarItem.md#color)
- [command](codearts_plugin_.StatusBarItem.md#command)
- [id](codearts_plugin_.StatusBarItem.md#id)
- [name](codearts_plugin_.StatusBarItem.md#name)
- [priority](codearts_plugin_.StatusBarItem.md#priority)
- [text](codearts_plugin_.StatusBarItem.md#text)
- [tooltip](codearts_plugin_.StatusBarItem.md#tooltip)

### Methods

- [dispose](codearts_plugin_.StatusBarItem.md#dispose)
- [hide](codearts_plugin_.StatusBarItem.md#hide)
- [show](codearts_plugin_.StatusBarItem.md#show)

## Properties

### accessibilityInformation

• **accessibilityInformation**: `undefined` \| [`AccessibilityInformation`](codearts_plugin_.AccessibilityInformation.md)

Accessibility information used when a screen reader interacts with this StatusBar item

#### Defined in

[index.d.ts:6381](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6381)

___

### alignment

• `Readonly` **alignment**: [`StatusBarAlignment`](../enums/codearts_plugin_.StatusBarAlignment.md)

The alignment of this item.

#### Defined in

[index.d.ts:6319](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6319)

___

### backgroundColor

• **backgroundColor**: `undefined` \| [`ThemeColor`](../classes/codearts_plugin_.ThemeColor.md)

The background color for this entry.

*Note*: only the following colors are supported:
* `new ThemeColor('statusBarItem.errorBackground')`
* `new ThemeColor('statusBarItem.warningBackground')`

More background colors may be supported in the future.

*Note*: when a background color is set, the statusbar may override
the `color` choice to ensure the entry is readable in all themes.

#### Defined in

[index.d.ts:6366](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6366)

___

### color

• **color**: `undefined` \| `string` \| [`ThemeColor`](../classes/codearts_plugin_.ThemeColor.md)

The foreground color for this entry.

#### Defined in

[index.d.ts:6352](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6352)

___

### command

• **command**: `undefined` \| `string` \| [`Command`](codearts_plugin_.Command.md)

[`Command`](codearts_plugin_.Command.md) or identifier of a command to run on click.

The command must be [known](../modules/codearts_plugin_.commands.md#getcommands).

Note that if this is a [`Command`](codearts_plugin_.Command.md) object, only the [`command`](codearts_plugin_.Command.md#command) and [`arguments`](codearts_plugin_.Command.md#arguments)
are used by the editor.

#### Defined in

[index.d.ts:6376](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6376)

___

### id

• `Readonly` **id**: `string`

The identifier of this item.

*Note*: if no identifier was provided by the [`createStatusBarItem`](../modules/codearts_plugin_.window.md#createstatusbaritem)
method, the identifier will match the [extension identifier](codearts_plugin_.Extension.md#id).

#### Defined in

[index.d.ts:6314](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6314)

___

### name

• **name**: `undefined` \| `string`

The name of the entry, like 'Python Language Indicator', 'Git Status' etc.
Try to keep the length of the name short, yet descriptive enough that
users can understand what the status bar item is about.

#### Defined in

[index.d.ts:6332](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6332)

___

### priority

• `Readonly` **priority**: `undefined` \| `number`

The priority of this item. Higher value means the item should
be shown more to the left.

#### Defined in

[index.d.ts:6325](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6325)

___

### text

• **text**: `string`

The text to show for the entry. You can embed icons in the text by leveraging the syntax:

`My text $(icon-name) contains icons like $(icon-name) this one.`

Where the icon-name is taken from the ThemeIcon [icon set](https://code.visualstudio.com/api/references/icons-in-labels#icon-listing), e.g.
`light-bulb`, `thumbsup`, `zap` etc.

#### Defined in

[index.d.ts:6342](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6342)

___

### tooltip

• **tooltip**: `undefined` \| `string` \| [`MarkdownString`](../classes/codearts_plugin_.MarkdownString.md)

The tooltip text when you hover over this entry.

#### Defined in

[index.d.ts:6347](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6347)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose and free associated resources. Call
[hide](codearts_plugin_.StatusBarItem.md#hide).

#### Returns

`void`

#### Defined in

[index.d.ts:6397](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6397)

___

### hide

▸ **hide**(): `void`

Hide the entry in the status bar.

#### Returns

`void`

#### Defined in

[index.d.ts:6391](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6391)

___

### show

▸ **show**(): `void`

Shows the entry in the status bar.

#### Returns

`void`

#### Defined in

[index.d.ts:6386](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L6386)
