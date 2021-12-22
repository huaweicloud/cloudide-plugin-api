**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TerminalExitStatus

# Interface: TerminalExitStatus

Represents how a terminal exited.

## Hierarchy

* **TerminalExitStatus**

## Index

### Properties

* [code](_index_d_._plugin_.terminalexitstatus.md#code)

## Properties

### code

• `Readonly` **code**: number \| undefined

*Defined in [index.d.ts:9560](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L9560)*

The exit code that a terminal exited with, it can have the following values:
- Zero: the terminal process or custom execution succeeded.
- Non-zero: the terminal process or custom execution failed.
- `undefined`: the user forcibly closed the terminal or a custom execution exited
  without providing an exit code.
