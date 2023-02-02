[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ExtensionTerminalOptions

# Interface: ExtensionTerminalOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).ExtensionTerminalOptions

Value-object describing what options a virtual process terminal should use.

## Table of contents

### Properties

- [color](codearts_plugin_.ExtensionTerminalOptions.md#color)
- [iconPath](codearts_plugin_.ExtensionTerminalOptions.md#iconpath)
- [isTransient](codearts_plugin_.ExtensionTerminalOptions.md#istransient)
- [location](codearts_plugin_.ExtensionTerminalOptions.md#location)
- [name](codearts_plugin_.ExtensionTerminalOptions.md#name)
- [pty](codearts_plugin_.ExtensionTerminalOptions.md#pty)

## Properties

### color

• `Optional` **color**: [`ThemeColor`](../classes/codearts_plugin_.ThemeColor.md)

The icon [ThemeColor](../classes/codearts_plugin_.ThemeColor.md) for the terminal.
The standard `terminal.ansi*` theme keys are
recommended for the best contrast and consistency across themes.

#### Defined in

[index.d.ts:11036](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L11036)

___

### iconPath

• `Optional` **iconPath**: [`Uri`](../classes/codearts_plugin_.Uri.md) \| [`ThemeIcon`](../classes/codearts_plugin_.ThemeIcon.md) \| { `dark`: [`Uri`](../classes/codearts_plugin_.Uri.md) ; `light`: [`Uri`](../classes/codearts_plugin_.Uri.md)  }

The icon path or [ThemeIcon](../classes/codearts_plugin_.ThemeIcon.md) for the terminal.

#### Defined in

[index.d.ts:11029](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L11029)

___

### isTransient

• `Optional` **isTransient**: `boolean`

Opt-out of the default terminal persistence on restart and reload.
This will only take effect when `terminal.integrated.enablePersistentSessions` is enabled.

#### Defined in

[index.d.ts:11047](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L11047)

___

### location

• `Optional` **location**: [`TerminalEditorLocationOptions`](codearts_plugin_.TerminalEditorLocationOptions.md) \| [`TerminalSplitLocationOptions`](codearts_plugin_.TerminalSplitLocationOptions.md) \| [`TerminalLocation`](../enums/codearts_plugin_.TerminalLocation.md)

The [TerminalLocation](../enums/codearts_plugin_.TerminalLocation.md) or [TerminalEditorLocationOptions](codearts_plugin_.TerminalEditorLocationOptions.md) or [TerminalSplitLocationOptions](codearts_plugin_.TerminalSplitLocationOptions.md) for the terminal.

#### Defined in

[index.d.ts:11041](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L11041)

___

### name

• **name**: `string`

A human-readable string which will be used to represent the terminal in the UI.

#### Defined in

[index.d.ts:11018](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L11018)

___

### pty

• **pty**: [`Pseudoterminal`](codearts_plugin_.Pseudoterminal.md)

An implementation of [Pseudoterminal](codearts_plugin_.Pseudoterminal.md) that allows an extension to
control a terminal.

#### Defined in

[index.d.ts:11024](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L11024)
