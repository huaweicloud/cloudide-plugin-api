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

[index.d.ts:7212](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7212)

___

### Never

• **Never** = ``3``

The terminal never comes to front when the task is executed.

#### Defined in

[index.d.ts:7223](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7223)

___

### Silent

• **Silent** = ``2``

Only brings the terminal to front if a problem is detected executing the task
(e.g. the task couldn't be started because).

#### Defined in

[index.d.ts:7218](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7218)
