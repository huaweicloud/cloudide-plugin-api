[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TerminalExitStatus

# Interface: TerminalExitStatus

["@codearts/plugin"](../modules/_codearts_plugin_.md).TerminalExitStatus

Represents how a terminal exited.

## Table of contents

### Properties

- [code](codearts_plugin_.TerminalExitStatus.md#code)

## Properties

### code

• `Readonly` **code**: `undefined` \| `number`

The exit code that a terminal exited with, it can have the following values:
- Zero: the terminal process or custom execution succeeded.
- Non-zero: the terminal process or custom execution failed.
- `undefined`: the user forcibly closed the terminal or a custom execution exited
  without providing an exit code.

#### Defined in

[index.d.ts:11422](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L11422)
