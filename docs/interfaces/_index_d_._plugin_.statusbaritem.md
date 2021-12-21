**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / StatusBarItem

# Interface: StatusBarItem

A status bar item is a status bar contribution that can
show text and icons and run a command on click.

## Hierarchy

* **StatusBarItem**

## Index

### Properties

* [accessibilityInformation](_index_d_._plugin_.statusbaritem.md#accessibilityinformation)
* [alignment](_index_d_._plugin_.statusbaritem.md#alignment)
* [backgroundColor](_index_d_._plugin_.statusbaritem.md#backgroundcolor)
* [color](_index_d_._plugin_.statusbaritem.md#color)
* [command](_index_d_._plugin_.statusbaritem.md#command)
* [priority](_index_d_._plugin_.statusbaritem.md#priority)
* [text](_index_d_._plugin_.statusbaritem.md#text)
* [tooltip](_index_d_._plugin_.statusbaritem.md#tooltip)

### Methods

* [dispose](_index_d_._plugin_.statusbaritem.md#dispose)
* [hide](_index_d_._plugin_.statusbaritem.md#hide)
* [show](_index_d_._plugin_.statusbaritem.md#show)

## Properties

### accessibilityInformation

• `Optional` **accessibilityInformation**: [AccessibilityInformation](_index_d_._plugin_.accessibilityinformation.md)

*Defined in [index.d.ts:5583](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5583)*

Accessibility information used when screen reader interacts with this StatusBar item

___

### alignment

• `Readonly` **alignment**: [StatusBarAlignment](../enums/_index_d_._plugin_.statusbaralignment.md)

*Defined in [index.d.ts:5530](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5530)*

The alignment of this item.

___

### backgroundColor

•  **backgroundColor**: [ThemeColor](../classes/_index_d_._plugin_.themecolor.md) \| undefined

*Defined in [index.d.ts:5568](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5568)*

The background color for this entry.

*Note*: only `new ThemeColor('statusBarItem.errorBackground')` is
supported for now. More background colors may be supported in the
future.

*Note*: when a background color is set, the statusbar may override
the `color` choice to ensure the entry is readable in all themes.

___

### color

•  **color**: string \| [ThemeColor](../classes/_index_d_._plugin_.themecolor.md) \| undefined

*Defined in [index.d.ts:5556](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5556)*

The foreground color for this entry.

___

### command

•  **command**: string \| [Command](_index_d_._plugin_.command.md) \| undefined

*Defined in [index.d.ts:5578](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5578)*

[`Command`](#Command) or identifier of a command to run on click.

The command must be [known](#commands.getCommands).

Note that if this is a [`Command`](#Command) object, only the [`command`](#Command.command) and [`arguments`](#Command.arguments)
are used by VS Code.

___

### priority

• `Optional` `Readonly` **priority**: number

*Defined in [index.d.ts:5536](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5536)*

The priority of this item. Higher value means the item should
be shown more to the left.

___

### text

•  **text**: string

*Defined in [index.d.ts:5546](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5546)*

The text to show for the entry. You can embed icons in the text by leveraging the syntax:

`My text $(icon-name) contains icons like $(icon-name) this one.`

Where the icon-name is taken from the ThemeIcon [icon set](https://code.visualstudio.com/api/references/icons-in-labels#icon-listing), e.g.
`light-bulb`, `thumbsup`, `zap` etc.

___

### tooltip

•  **tooltip**: string \| undefined

*Defined in [index.d.ts:5551](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5551)*

The tooltip text when you hover over this entry.

## Methods

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:5599](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5599)*

Dispose and free associated resources. Call
[hide](#StatusBarItem.hide).

**Returns:** void

___

### hide

▸ **hide**(): void

*Defined in [index.d.ts:5593](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5593)*

Hide the entry in the status bar.

**Returns:** void

___

### show

▸ **show**(): void

*Defined in [index.d.ts:5588](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5588)*

Shows the entry in the status bar.

**Returns:** void
