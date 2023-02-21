[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TaskPanelKind

# Enumeration: TaskPanelKind

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TaskPanelKind

Controls how the task channel is used between tasks

## Table of contents

### Enumeration Members

- [Dedicated](cloudide_plugin_.TaskPanelKind.md#dedicated)
- [New](cloudide_plugin_.TaskPanelKind.md#new)
- [Shared](cloudide_plugin_.TaskPanelKind.md#shared)

## Enumeration Members

### Dedicated

• **Dedicated** = ``2``

Uses a dedicated panel for this tasks. The panel is not
shared with other tasks.

#### Defined in

[index.d.ts:10449](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10449)

___

### New

• **New** = ``3``

Creates a new panel whenever this task is executed.

#### Defined in

[index.d.ts:10452](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10452)

___

### Shared

• **Shared** = ``1``

Shares a panel with other tasks. This is the default.

#### Defined in

[index.d.ts:10443](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10443)
