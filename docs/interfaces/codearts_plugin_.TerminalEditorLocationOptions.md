[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TerminalEditorLocationOptions

# Interface: TerminalEditorLocationOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).TerminalEditorLocationOptions

Assumes a [TerminalLocation](../enums/codearts_plugin_.TerminalLocation.md) of editor and allows specifying a [ViewColumn](../enums/codearts_plugin_.ViewColumn.md) and
[preserveFocus](codearts_plugin_.TerminalEditorLocationOptions.md#preservefocus) property

## Table of contents

### Properties

- [preserveFocus](codearts_plugin_.TerminalEditorLocationOptions.md#preservefocus)
- [viewColumn](codearts_plugin_.TerminalEditorLocationOptions.md#viewcolumn)

## Properties

### preserveFocus

• `Optional` **preserveFocus**: `boolean`

An optional flag that when `true` will stop the [Terminal](codearts_plugin_.Terminal.md) from taking focus.

#### Defined in

[index.d.ts:6607](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6607)

___

### viewColumn

• **viewColumn**: [`ViewColumn`](../enums/codearts_plugin_.ViewColumn.md)

A view column in which the [terminal](codearts_plugin_.Terminal.md) should be shown in the editor area.
Use [active](../enums/codearts_plugin_.ViewColumn.md#active) to open in the active editor group, other values are
adjusted to be `Min(column, columnCount + 1)`, the
[active](../enums/codearts_plugin_.ViewColumn.md#active)-column is not adjusted. Use
[`Beside`](../enums/codearts_plugin_.ViewColumn.md#beside) to open the editor to the side of the currently active one.

#### Defined in

[index.d.ts:6603](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6603)
