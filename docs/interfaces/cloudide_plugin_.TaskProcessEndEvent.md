[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TaskProcessEndEvent

# Interface: TaskProcessEndEvent

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TaskProcessEndEvent

An event signaling the end of a process execution
triggered through a task

## Table of contents

### Properties

- [execution](cloudide_plugin_.TaskProcessEndEvent.md#execution)
- [exitCode](cloudide_plugin_.TaskProcessEndEvent.md#exitcode)

## Properties

### execution

• **execution**: [`TaskExecution`](cloudide_plugin_.TaskExecution.md)

The task execution for which the process got started.

#### Defined in

[index.d.ts:10655](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10655)

___

### exitCode

• **exitCode**: `number`

The process's exit code.

#### Defined in

[index.d.ts:10660](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10660)
