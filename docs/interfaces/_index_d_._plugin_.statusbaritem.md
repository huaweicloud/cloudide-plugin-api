**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / StatusBarItem

# Interface: StatusBarItem

A status bar item is a status bar contribution that can
show text and icons and run a command on click.

## Hierarchy

* **StatusBarItem**

## Index

### Properties

* [alignment](_index_d_._plugin_.statusbaritem.md#alignment)
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

### alignment

• `Readonly` **alignment**: [StatusBarAlignment](../enums/_index_d_._plugin_.statusbaralignment.md)

*Defined in [index.d.ts:5218](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5218)*

The alignment of this item.

___

### color

•  **color**: string \| [ThemeColor](../classes/_index_d_._plugin_.themecolor.md) \| undefined

*Defined in [index.d.ts:5244](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5244)*

The foreground color for this entry.

___

### command

•  **command**: string \| [Command](_index_d_._plugin_.command.md) \| undefined

*Defined in [index.d.ts:5254](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5254)*

[`Command`](#Command) or identifier of a command to run on click.

The command must be [known](#commands.getCommands).

Note that if this is a [`Command`](#Command) object, only the [`command`](#Command.command) and [`arguments`](#Command.arguments)
are used by VS Code.

___

### priority

• `Optional` `Readonly` **priority**: number

*Defined in [index.d.ts:5224](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5224)*

The priority of this item. Higher value means the item should
be shown more to the left.

___

### text

•  **text**: string

*Defined in [index.d.ts:5234](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5234)*

The text to show for the entry. You can embed icons in the text by leveraging the syntax:

`My text $(icon-name) contains icons like $(icon-name) this one.`

Where the icon-name is taken from the [codicon](https://microsoft.github.io/vscode-codicons/dist/codicon.html) icon set, e.g.
`light-bulb`, `thumbsup`, `zap` etc.

___

### tooltip

•  **tooltip**: string \| undefined

*Defined in [index.d.ts:5239](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5239)*

The tooltip text when you hover over this entry.

## Methods

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:5270](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5270)*

Dispose and free associated resources. Call
[hide](#StatusBarItem.hide).

**Returns:** void

___

### hide

▸ **hide**(): void

*Defined in [index.d.ts:5264](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5264)*

Hide the entry in the status bar.

**Returns:** void

___

### show

▸ **show**(): void

*Defined in [index.d.ts:5259](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5259)*

Shows the entry in the status bar.

**Returns:** void
