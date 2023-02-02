[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TaskProcessStartEvent

# Interface: TaskProcessStartEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).TaskProcessStartEvent

An event signaling the start of a process execution
triggered through a task

## Table of contents

### Properties

- [execution](codearts_plugin_.TaskProcessStartEvent.md#execution)
- [processId](codearts_plugin_.TaskProcessStartEvent.md#processid)

## Properties

### execution

• `Readonly` **execution**: [`TaskExecution`](codearts_plugin_.TaskExecution.md)

The task execution for which the process got started.

#### Defined in

[index.d.ts:7689](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7689)

___

### processId

• `Readonly` **processId**: `number`

The underlying process id.

#### Defined in

[index.d.ts:7694](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7694)
