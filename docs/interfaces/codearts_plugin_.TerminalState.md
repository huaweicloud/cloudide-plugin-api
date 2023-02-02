[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TerminalState

# Interface: TerminalState

["@codearts/plugin"](../modules/_codearts_plugin_.md).TerminalState

Represents the state of a [Terminal](codearts_plugin_.Terminal.md).

## Table of contents

### Properties

- [isInteractedWith](codearts_plugin_.TerminalState.md#isinteractedwith)

## Properties

### isInteractedWith

• `Readonly` **isInteractedWith**: `boolean`

Whether the [Terminal](codearts_plugin_.Terminal.md) has been interacted with. Interaction means that the
terminal has sent data to the process which depending on the terminal's _mode_. By
default input is sent when a key is pressed or when a command or extension sends text,
but based on the terminal's mode it can also happen on:

- a pointer click event
- a pointer scroll event
- a pointer move event
- terminal focus in/out

For more information on events that can send data see "DEC Private Mode Set (DECSET)" on
https://invisible-island.net/xterm/ctlseqs/ctlseqs.html

#### Defined in

[index.d.ts:6601](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L6601)
