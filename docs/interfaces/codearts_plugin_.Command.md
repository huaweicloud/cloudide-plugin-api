[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Command

# Interface: Command

["@codearts/plugin"](../modules/_codearts_plugin_.md).Command

Represents a reference to a command. Provides a title which
will be used to represent a command in the UI and, optionally,
an array of arguments which will be passed to the command handler
function when invoked.

## Table of contents

### Properties

- [arguments](codearts_plugin_.Command.md#arguments)
- [command](codearts_plugin_.Command.md#command)
- [title](codearts_plugin_.Command.md#title)
- [tooltip](codearts_plugin_.Command.md#tooltip)

## Properties

### arguments

• `Optional` **arguments**: `any`[]

Arguments that the command handler should be
invoked with.

#### Defined in

[index.d.ts:48](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L48)

___

### command

• **command**: `string`

The identifier of the actual command handler.

**`See`**

[registerCommand](../modules/codearts_plugin_.commands.md#registercommand)

#### Defined in

[index.d.ts:37](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L37)

___

### title

• **title**: `string`

Title of the command, like `save`.

#### Defined in

[index.d.ts:31](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L31)

___

### tooltip

• `Optional` **tooltip**: `string`

A tooltip for the command, when represented in the UI.

#### Defined in

[index.d.ts:42](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L42)
