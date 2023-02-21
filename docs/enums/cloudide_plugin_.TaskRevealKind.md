[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TaskRevealKind

# Enumeration: TaskRevealKind

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TaskRevealKind

Controls the behaviour of the terminal's visibility.

## Table of contents

### Enumeration Members

- [Always](cloudide_plugin_.TaskRevealKind.md#always)
- [Never](cloudide_plugin_.TaskRevealKind.md#never)
- [Silent](cloudide_plugin_.TaskRevealKind.md#silent)

## Enumeration Members

### Always

• **Always** = ``1``

Always brings the terminal to front if the task is executed.

#### Defined in

[index.d.ts:10427](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10427)

___

### Never

• **Never** = ``3``

The terminal never comes to front when the task is executed.

#### Defined in

[index.d.ts:10436](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10436)

___

### Silent

• **Silent** = ``2``

Only brings the terminal to front if a problem is detected executing the task
(e.g. the task couldn't be started because).

#### Defined in

[index.d.ts:10433](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10433)
