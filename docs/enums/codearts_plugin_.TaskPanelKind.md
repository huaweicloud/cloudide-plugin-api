[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TaskPanelKind

# Enumeration: TaskPanelKind

["@codearts/plugin"](../modules/_codearts_plugin_.md).TaskPanelKind

Controls how the task channel is used between tasks

## Table of contents

### Enumeration Members

- [Dedicated](codearts_plugin_.TaskPanelKind.md#dedicated)
- [New](codearts_plugin_.TaskPanelKind.md#new)
- [Shared](codearts_plugin_.TaskPanelKind.md#shared)

## Enumeration Members

### Dedicated

• **Dedicated** = ``2``

Uses a dedicated panel for this tasks. The panel is not
shared with other tasks.

#### Defined in

[index.d.ts:7113](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7113)

___

### New

• **New** = ``3``

Creates a new panel whenever this task is executed.

#### Defined in

[index.d.ts:7118](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7118)

___

### Shared

• **Shared** = ``1``

Shares a panel with other tasks. This is the default.

#### Defined in

[index.d.ts:7107](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7107)
