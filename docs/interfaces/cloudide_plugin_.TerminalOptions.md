[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TerminalOptions

# Interface: TerminalOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TerminalOptions

Options to create terminal widget.

## Table of contents

### Properties

- [attributes](cloudide_plugin_.TerminalOptions.md#attributes)
- [cwd](cloudide_plugin_.TerminalOptions.md#cwd)
- [env](cloudide_plugin_.TerminalOptions.md#env)
- [name](cloudide_plugin_.TerminalOptions.md#name)
- [shellArgs](cloudide_plugin_.TerminalOptions.md#shellargs)
- [shellPath](cloudide_plugin_.TerminalOptions.md#shellpath)

## Properties

### attributes

• `Optional` **attributes**: `Object`

Terminal attributes. Can be useful to apply some implementation specific information.

#### Index signature

▪ [key: `string`]: `string` \| ``null``

#### Defined in

[index.d.ts:2809](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2809)

___

### cwd

• `Optional` **cwd**: `any`

Current working directory.

#### Defined in

[index.d.ts:2799](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2799)

___

### env

• `Optional` **env**: `Object`

Environment variables for terminal in format key - value.

#### Index signature

▪ [key: `string`]: `string` \| ``null``

#### Defined in

[index.d.ts:2804](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2804)

___

### name

• `Optional` **name**: `string`

Human readable representation of the terminal in the UI.

#### Defined in

[index.d.ts:2784](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2784)

___

### shellArgs

• `Optional` **shellArgs**: `string`[]

Arguments to configure executable shell. For example ["-l"] - run shell without login.

#### Defined in

[index.d.ts:2794](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2794)

___

### shellPath

• `Optional` **shellPath**: `string`

Path to the executable shell. For example "/bin/bash", "bash", "sh".

#### Defined in

[index.d.ts:2789](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2789)
