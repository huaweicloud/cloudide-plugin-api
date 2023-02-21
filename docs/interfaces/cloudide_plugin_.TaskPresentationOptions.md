[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TaskPresentationOptions

# Interface: TaskPresentationOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TaskPresentationOptions

## Table of contents

### Properties

- [echo](cloudide_plugin_.TaskPresentationOptions.md#echo)
- [focus](cloudide_plugin_.TaskPresentationOptions.md#focus)
- [panel](cloudide_plugin_.TaskPresentationOptions.md#panel)
- [reveal](cloudide_plugin_.TaskPresentationOptions.md#reveal)
- [showReuseMessage](cloudide_plugin_.TaskPresentationOptions.md#showreusemessage)

## Properties

### echo

• `Optional` **echo**: `boolean`

Controls whether the command associated with the task is echoed
in the user interface.

#### Defined in

[index.d.ts:10466](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10466)

___

### focus

• `Optional` **focus**: `boolean`

Controls whether the panel showing the task output is taking focus.

#### Defined in

[index.d.ts:10469](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10469)

___

### panel

• `Optional` **panel**: [`TaskPanelKind`](../enums/cloudide_plugin_.TaskPanelKind.md)

Controls if the task panel is used for this task only (dedicated),
shared between tasks (shared) or if a new panel is created on
every task execution (new). Defaults to `TaskInstanceKind.Shared`

#### Defined in

[index.d.ts:10476](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10476)

___

### reveal

• `Optional` **reveal**: [`TaskRevealKind`](../enums/cloudide_plugin_.TaskRevealKind.md)

Controls whether the task output is reveal in the user interface.
Defaults to `RevealKind.Always`.

#### Defined in

[index.d.ts:10460](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10460)

___

### showReuseMessage

• `Optional` **showReuseMessage**: `boolean`

Controls whether to show the "Terminal will be reused by tasks, press any key to close it" message.

#### Defined in

[index.d.ts:10479](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10479)
