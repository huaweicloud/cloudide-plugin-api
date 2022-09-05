[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ProcessExecution

# Class: ProcessExecution

["@codearts/plugin"](../modules/_codearts_plugin_.md).ProcessExecution

The execution of a task happens as an external process
without shell interaction.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.ProcessExecution.md#constructor)

### Properties

- [args](codearts_plugin_.ProcessExecution.md#args)
- [options](codearts_plugin_.ProcessExecution.md#options)
- [process](codearts_plugin_.ProcessExecution.md#process)

## Constructors

### constructor

• **new ProcessExecution**(`process`, `options?`)

Creates a process execution.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `process` | `string` | The process to start. |
| `options?` | [`ProcessExecutionOptions`](../interfaces/codearts_plugin_.ProcessExecutionOptions.md) | Optional options for the started process. |

#### Defined in

[index.d.ts:7258](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7258)

• **new ProcessExecution**(`process`, `args`, `options?`)

Creates a process execution.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `process` | `string` | The process to start. |
| `args` | `string`[] | Arguments to be passed to the process. |
| `options?` | [`ProcessExecutionOptions`](../interfaces/codearts_plugin_.ProcessExecutionOptions.md) | Optional options for the started process. |

#### Defined in

[index.d.ts:7267](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7267)

## Properties

### args

• **args**: `string`[]

The arguments passed to the process. Defaults to an empty array.

#### Defined in

[index.d.ts:7277](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7277)

___

### options

• `Optional` **options**: [`ProcessExecutionOptions`](../interfaces/codearts_plugin_.ProcessExecutionOptions.md)

The process options used when the process is executed.
Defaults to undefined.

#### Defined in

[index.d.ts:7283](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7283)

___

### process

• **process**: `string`

The process to be executed.

#### Defined in

[index.d.ts:7272](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7272)
