[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CustomExecution

# Class: CustomExecution

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CustomExecution

Class used to execute an extension callback as a task.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.CustomExecution.md#constructor)

### Properties

- [callback](cloudide_plugin_.CustomExecution.md#callback)

## Constructors

### constructor

• **new CustomExecution**(`callback`)

Constructs a CustomExecution task object. The callback will be executed when the task is run, at which point the
extension should return the Pseudoterminal it will "run in". The task should wait to do further execution until
[Pseudoterminal.open](#Pseudoterminal.open) is called. Task cancellation should be handled using
[Pseudoterminal.close](#Pseudoterminal.close). When the task is complete fire
[Pseudoterminal.onDidClose](#Pseudoterminal.onDidClose).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`resolvedDefinition`: [`TaskDefinition`](../interfaces/cloudide_plugin_.TaskDefinition.md)) => [`Thenable`](../interfaces/Thenable.md)<[`Pseudoterminal`](../interfaces/cloudide_plugin_.Pseudoterminal.md)\> | The callback that will be called when the task is started by a user. Any ${} style variables that were in the task definition will be resolved and passed into the callback as `resolvedDefinition`. |

#### Defined in

[index.d.ts:10394](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10394)

## Properties

### callback

• `Readonly` **callback**: `any`

#### Defined in

[index.d.ts:10396](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10396)
