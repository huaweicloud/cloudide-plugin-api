[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TaskPresentationOptions

# Interface: TaskPresentationOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).TaskPresentationOptions

Controls how the task is presented in the UI.

## Table of contents

### Properties

- [clear](codearts_plugin_.TaskPresentationOptions.md#clear)
- [echo](codearts_plugin_.TaskPresentationOptions.md#echo)
- [focus](codearts_plugin_.TaskPresentationOptions.md#focus)
- [panel](codearts_plugin_.TaskPresentationOptions.md#panel)
- [reveal](codearts_plugin_.TaskPresentationOptions.md#reveal)
- [showReuseMessage](codearts_plugin_.TaskPresentationOptions.md#showreusemessage)

## Properties

### clear

• `Optional` **clear**: `boolean`

Controls whether the terminal is cleared before executing the task.

#### Defined in

[index.d.ts:7157](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7157)

___

### echo

• `Optional` **echo**: `boolean`

Controls whether the command associated with the task is echoed
in the user interface.

#### Defined in

[index.d.ts:7135](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7135)

___

### focus

• `Optional` **focus**: `boolean`

Controls whether the panel showing the task output is taking focus.

#### Defined in

[index.d.ts:7140](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7140)

___

### panel

• `Optional` **panel**: [`TaskPanelKind`](../enums/codearts_plugin_.TaskPanelKind.md)

Controls if the task panel is used for this task only (dedicated),
shared between tasks (shared) or if a new panel is created on
every task execution (new). Defaults to `TaskInstanceKind.Shared`

#### Defined in

[index.d.ts:7147](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7147)

___

### reveal

• `Optional` **reveal**: [`TaskRevealKind`](../enums/codearts_plugin_.TaskRevealKind.md)

Controls whether the task output is reveal in the user interface.
Defaults to `RevealKind.Always`.

#### Defined in

[index.d.ts:7129](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7129)

___

### showReuseMessage

• `Optional` **showReuseMessage**: `boolean`

Controls whether to show the "Terminal will be reused by tasks, press any key to close it" message.

#### Defined in

[index.d.ts:7152](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7152)
