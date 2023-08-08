[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TaskExecution

# Interface: TaskExecution

["@codearts/plugin"](../modules/_codearts_plugin_.md).TaskExecution

An object representing an executed Task. It can be used
to terminate a task.

This interface is not intended to be implemented.

## Table of contents

### Properties

- [task](codearts_plugin_.TaskExecution.md#task)

### Methods

- [terminate](codearts_plugin_.TaskExecution.md#terminate)

## Properties

### task

• **task**: [`Task`](../classes/codearts_plugin_.Task.md)

The task that got started.

#### Defined in

[index.d.ts:7721](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7721)

## Methods

### terminate

▸ **terminate**(): `void`

Terminates the task execution.

#### Returns

`void`

#### Defined in

[index.d.ts:7726](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L7726)
