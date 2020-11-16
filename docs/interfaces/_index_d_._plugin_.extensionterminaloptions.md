**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ExtensionTerminalOptions

# Interface: ExtensionTerminalOptions

Value-object describing what options a virtual process terminal should use.

## Hierarchy

* **ExtensionTerminalOptions**

## Index

### Properties

* [name](_index_d_._plugin_.extensionterminaloptions.md#name)
* [pty](_index_d_._plugin_.extensionterminaloptions.md#pty)

## Properties

### name

•  **name**: string

*Defined in [index.d.ts:8126](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8126)*

A human-readable string which will be used to represent the terminal in the UI.

___

### pty

•  **pty**: [Pseudoterminal](_index_d_._plugin_.pseudoterminal.md)

*Defined in [index.d.ts:8132](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8132)*

An implementation of [Pseudoterminal](#Pseudoterminal) that allows an extension to
control a terminal.
