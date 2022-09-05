[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TaskRevealKind

# Enumeration: TaskRevealKind

["@codearts/plugin"](../modules/_codearts_plugin_.md).TaskRevealKind

Controls the behaviour of the terminal's visibility.

## Table of contents

### Enumeration Members

- [Always](codearts_plugin_.TaskRevealKind.md#always)
- [Never](codearts_plugin_.TaskRevealKind.md#never)
- [Silent](codearts_plugin_.TaskRevealKind.md#silent)

## Enumeration Members

### Always

• **Always** = ``1``

Always brings the terminal to front if the task is executed.

#### Defined in

[index.d.ts:7085](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7085)

___

### Never

• **Never** = ``3``

The terminal never comes to front when the task is executed.

#### Defined in

[index.d.ts:7096](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7096)

___

### Silent

• **Silent** = ``2``

Only brings the terminal to front if a problem is detected executing the task
(e.g. the task couldn't be started because).

#### Defined in

[index.d.ts:7091](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7091)
