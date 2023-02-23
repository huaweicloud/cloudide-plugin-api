[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Command

# Interface: Command

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Command

Command represents a particular invocation of a registered command.

## Table of contents

### Properties

- [arguments](cloudide_plugin_.Command.md#arguments)
- [command](cloudide_plugin_.Command.md#command)
- [id](cloudide_plugin_.Command.md#id)
- [label](cloudide_plugin_.Command.md#label)
- [title](cloudide_plugin_.Command.md#title)
- [tooltip](cloudide_plugin_.Command.md#tooltip)

## Properties

### arguments

• `Optional` **arguments**: `any`[]

Arguments that the command handler should be
invoked with.

#### Defined in

[index.d.ts:290](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L290)

___

### command

• `Optional` **command**: `string`

The identifier of the actual command handler.

#### Defined in

[index.d.ts:277](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L277)

___

### id

• `Optional` **id**: `string`

**`Deprecated`**

use command instead

#### Defined in

[index.d.ts:295](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L295)

___

### label

• `Optional` **label**: `string`

**`Deprecated`**

use title instead

#### Defined in

[index.d.ts:299](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L299)

___

### title

• `Optional` **title**: `string`

Title of the command invocation, like "Add local variable 'foo'".

#### Defined in

[index.d.ts:281](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L281)

___

### tooltip

• `Optional` **tooltip**: `string`

A tooltip for for command, when represented in the UI.

#### Defined in

[index.d.ts:285](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L285)
