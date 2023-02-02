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

[index.d.ts:7168](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7168)

___

### New

• **New** = ``3``

Creates a new panel whenever this task is executed.

#### Defined in

[index.d.ts:7173](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7173)

___

### Shared

• **Shared** = ``1``

Shares a panel with other tasks. This is the default.

#### Defined in

[index.d.ts:7162](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7162)
