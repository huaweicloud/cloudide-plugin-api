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

[index.d.ts:7211](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7211)

___

### New

• **New** = ``3``

Creates a new panel whenever this task is executed.

#### Defined in

[index.d.ts:7216](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7216)

___

### Shared

• **Shared** = ``1``

Shares a panel with other tasks. This is the default.

#### Defined in

[index.d.ts:7205](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7205)
