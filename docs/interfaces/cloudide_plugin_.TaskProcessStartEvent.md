[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TaskProcessStartEvent

# Interface: TaskProcessStartEvent

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TaskProcessStartEvent

An event signaling the start of a process execution
triggered through a task

## Table of contents

### Properties

- [execution](cloudide_plugin_.TaskProcessStartEvent.md#execution)
- [processId](cloudide_plugin_.TaskProcessStartEvent.md#processid)

## Properties

### execution

• **execution**: [`TaskExecution`](cloudide_plugin_.TaskExecution.md)

The task execution for which the process got started.

#### Defined in

[index.d.ts:10638](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10638)

___

### processId

• **processId**: `number`

The underlying process id.

#### Defined in

[index.d.ts:10643](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10643)
