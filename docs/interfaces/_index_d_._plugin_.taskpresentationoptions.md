**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TaskPresentationOptions

# Interface: TaskPresentationOptions

Controls how the task is presented in the UI.

## Hierarchy

* **TaskPresentationOptions**

## Index

### Properties

* [clear](_index_d_._plugin_.taskpresentationoptions.md#clear)
* [echo](_index_d_._plugin_.taskpresentationoptions.md#echo)
* [focus](_index_d_._plugin_.taskpresentationoptions.md#focus)
* [panel](_index_d_._plugin_.taskpresentationoptions.md#panel)
* [reveal](_index_d_._plugin_.taskpresentationoptions.md#reveal)
* [showReuseMessage](_index_d_._plugin_.taskpresentationoptions.md#showreusemessage)

## Properties

### clear

• `Optional` **clear**: boolean

*Defined in [index.d.ts:6232](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6232)*

Controls whether the terminal is cleared before executing the task.

___

### echo

• `Optional` **echo**: boolean

*Defined in [index.d.ts:6210](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6210)*

Controls whether the command associated with the task is echoed
in the user interface.

___

### focus

• `Optional` **focus**: boolean

*Defined in [index.d.ts:6215](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6215)*

Controls whether the panel showing the task output is taking focus.

___

### panel

• `Optional` **panel**: [TaskPanelKind](../enums/_index_d_._plugin_.taskpanelkind.md)

*Defined in [index.d.ts:6222](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6222)*

Controls if the task panel is used for this task only (dedicated),
shared between tasks (shared) or if a new panel is created on
every task execution (new). Defaults to `TaskInstanceKind.Shared`

___

### reveal

• `Optional` **reveal**: [TaskRevealKind](../enums/_index_d_._plugin_.taskrevealkind.md)

*Defined in [index.d.ts:6204](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6204)*

Controls whether the task output is reveal in the user interface.
Defaults to `RevealKind.Always`.

___

### showReuseMessage

• `Optional` **showReuseMessage**: boolean

*Defined in [index.d.ts:6227](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L6227)*

Controls whether to show the "Terminal will be reused by tasks, press any key to close it" message.
