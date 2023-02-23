[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ProcessExecution

# Class: ProcessExecution

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ProcessExecution

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.ProcessExecution.md#constructor)

### Properties

- [args](cloudide_plugin_.ProcessExecution.md#args)
- [options](cloudide_plugin_.ProcessExecution.md#options)
- [process](cloudide_plugin_.ProcessExecution.md#process)

## Constructors

### constructor

• **new ProcessExecution**(`process`, `options?`)

Creates a process execution.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `process` | `string` | The process to start. |
| `options?` | [`ProcessExecutionOptions`](../interfaces/cloudide_plugin_.ProcessExecutionOptions.md) | Optional options for the started process. |

#### Defined in

[index.d.ts:10335](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10335)

• **new ProcessExecution**(`process`, `args`, `options?`)

Creates a process execution.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `process` | `string` | The process to start. |
| `args` | `string`[] | Arguments to be passed to the process. |
| `options?` | [`ProcessExecutionOptions`](../interfaces/cloudide_plugin_.ProcessExecutionOptions.md) | Optional options for the started process. |

#### Defined in

[index.d.ts:10344](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10344)

## Properties

### args

• **args**: `string`[]

The arguments passed to the process. Defaults to an empty array.

#### Defined in

[index.d.ts:10350](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10350)

___

### options

• `Optional` **options**: [`ProcessExecutionOptions`](../interfaces/cloudide_plugin_.ProcessExecutionOptions.md)

The process options used when the process is executed.
Defaults to undefined.

#### Defined in

[index.d.ts:10356](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10356)

___

### process

• **process**: `string`

The process to be executed.

#### Defined in

[index.d.ts:10347](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10347)
