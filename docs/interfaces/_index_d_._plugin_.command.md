**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Command

# Interface: Command

Represents a reference to a command. Provides a title which
will be used to represent a command in the UI and, optionally,
an array of arguments which will be passed to the command handler
function when invoked.

## Hierarchy

* **Command**

## Index

### Properties

* [arguments](_index_d_._plugin_.command.md#arguments)
* [command](_index_d_._plugin_.command.md#command)
* [title](_index_d_._plugin_.command.md#title)
* [tooltip](_index_d_._plugin_.command.md#tooltip)

## Properties

### arguments

• `Optional` **arguments**: any[]

*Defined in [index.d.ts:158](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L158)*

Arguments that the command handler should be
invoked with.

___

### command

•  **command**: string

*Defined in [index.d.ts:147](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L147)*

The identifier of the actual command handler.

**`see`** [commands.registerCommand](#commands.registerCommand).

___

### title

•  **title**: string

*Defined in [index.d.ts:141](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L141)*

Title of the command, like `save`.

___

### tooltip

• `Optional` **tooltip**: string

*Defined in [index.d.ts:152](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L152)*

A tooltip for the command, when represented in the UI.
