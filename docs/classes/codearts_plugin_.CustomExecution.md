[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CustomExecution

# Class: CustomExecution

["@codearts/plugin"](../modules/_codearts_plugin_.md).CustomExecution

Class used to execute an extension callback as a task.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.CustomExecution.md#constructor)

## Constructors

### constructor

• **new CustomExecution**(`callback`)

Constructs a CustomExecution task object. The callback will be executed when the task is run, at which point the
extension should return the Pseudoterminal it will "run in". The task should wait to do further execution until
[open](../interfaces/codearts_plugin_.Pseudoterminal.md#open) is called. Task cancellation should be handled using
[close](../interfaces/codearts_plugin_.Pseudoterminal.md#close). When the task is complete fire
[onDidClose](../interfaces/codearts_plugin_.Pseudoterminal.md#ondidclose).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`resolvedDefinition`: [`TaskDefinition`](../interfaces/codearts_plugin_.TaskDefinition.md)) => [`Thenable`](../interfaces/Thenable.md)<[`Pseudoterminal`](../interfaces/codearts_plugin_.Pseudoterminal.md)\> | The callback that will be called when the task is started by a user. Any ${} style variables that were in the task definition will be resolved and passed into the callback as `resolvedDefinition`. |

#### Defined in

[index.d.ts:7456](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7456)
