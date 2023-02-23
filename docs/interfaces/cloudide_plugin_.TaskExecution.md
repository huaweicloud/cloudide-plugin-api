[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TaskExecution

# Interface: TaskExecution

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TaskExecution

An object representing an executed Task. It can be used
to terminate a task.

This interface is not intended to be implemented.

## Table of contents

### Properties

- [task](cloudide_plugin_.TaskExecution.md#task)

### Methods

- [terminate](cloudide_plugin_.TaskExecution.md#terminate)

## Properties

### task

• **task**: [`Task`](../classes/cloudide_plugin_.Task.md)

The task that got started.

#### Defined in

[index.d.ts:10598](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10598)

## Methods

### terminate

▸ **terminate**(): `void`

Terminates the task execution.

#### Returns

`void`

#### Defined in

[index.d.ts:10603](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10603)
