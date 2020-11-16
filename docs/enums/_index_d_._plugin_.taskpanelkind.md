**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TaskPanelKind

# Enumeration: TaskPanelKind

Controls how the task channel is used between tasks

## Index

### Enumeration members

* [Dedicated](_index_d_._plugin_.taskpanelkind.md#dedicated)
* [New](_index_d_._plugin_.taskpanelkind.md#new)
* [Shared](_index_d_._plugin_.taskpanelkind.md#shared)

## Enumeration members

### Dedicated

•  **Dedicated**:  = 2

*Defined in [index.d.ts:5586](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5586)*

Uses a dedicated panel for this tasks. The panel is not
shared with other tasks.

___

### New

•  **New**:  = 3

*Defined in [index.d.ts:5591](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5591)*

Creates a new panel whenever this task is executed.

___

### Shared

•  **Shared**:  = 1

*Defined in [index.d.ts:5580](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5580)*

Shares a panel with other tasks. This is the default.
