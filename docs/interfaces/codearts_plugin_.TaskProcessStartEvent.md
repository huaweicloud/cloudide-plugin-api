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

[index.d.ts:7719](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7719)

___

### processId

• `Readonly` **processId**: `number`

The underlying process id.

#### Defined in

[index.d.ts:7724](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7724)
