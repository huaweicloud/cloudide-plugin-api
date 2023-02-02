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

[index.d.ts:7313](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7313)

• **new ProcessExecution**(`process`, `args`, `options?`)

Creates a process execution.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `process` | `string` | The process to start. |
| `args` | `string`[] | Arguments to be passed to the process. |
| `options?` | [`ProcessExecutionOptions`](../interfaces/codearts_plugin_.ProcessExecutionOptions.md) | Optional options for the started process. |

#### Defined in

[index.d.ts:7322](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7322)

## Properties

### args

• **args**: `string`[]

The arguments passed to the process. Defaults to an empty array.

#### Defined in

[index.d.ts:7332](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7332)

___

### options

• `Optional` **options**: [`ProcessExecutionOptions`](../interfaces/codearts_plugin_.ProcessExecutionOptions.md)

The process options used when the process is executed.
Defaults to undefined.

#### Defined in

[index.d.ts:7338](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7338)

___

### process

• **process**: `string`

The process to be executed.

#### Defined in

[index.d.ts:7327](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7327)
