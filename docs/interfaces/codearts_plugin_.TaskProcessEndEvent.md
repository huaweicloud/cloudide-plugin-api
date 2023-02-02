[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TaskProcessEndEvent

# Interface: TaskProcessEndEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).TaskProcessEndEvent

An event signaling the end of a process execution
triggered through a task

## Table of contents

### Properties

- [execution](codearts_plugin_.TaskProcessEndEvent.md#execution)
- [exitCode](codearts_plugin_.TaskProcessEndEvent.md#exitcode)

## Properties

### execution

• `Readonly` **execution**: [`TaskExecution`](codearts_plugin_.TaskExecution.md)

The task execution for which the process got started.

#### Defined in

[index.d.ts:7706](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7706)

___

### exitCode

• `Readonly` **exitCode**: `undefined` \| `number`

The process's exit code. Will be `undefined` when the task is terminated.

#### Defined in

[index.d.ts:7711](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7711)
