[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Task

# Class: Task

["@codearts/plugin"](../modules/_codearts_plugin_.md).Task

## Table of contents

### Constructors

- [constructor](codearts_plugin_.Task.md#constructor)

### Properties

- [definition](codearts_plugin_.Task.md#definition)
- [detail](codearts_plugin_.Task.md#detail)
- [execution](codearts_plugin_.Task.md#execution)
- [group](codearts_plugin_.Task.md#group)
- [isBackground](codearts_plugin_.Task.md#isbackground)
- [name](codearts_plugin_.Task.md#name)
- [presentationOptions](codearts_plugin_.Task.md#presentationoptions)
- [problemMatchers](codearts_plugin_.Task.md#problemmatchers)
- [runOptions](codearts_plugin_.Task.md#runoptions)
- [scope](codearts_plugin_.Task.md#scope)
- [source](codearts_plugin_.Task.md#source)

## Constructors

### constructor

• **new Task**(`taskDefinition`, `scope`, `name`, `source`, `execution?`, `problemMatchers?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskDefinition` | [`TaskDefinition`](../interfaces/codearts_plugin_.TaskDefinition.md) |  |
| `scope` | [`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) \| [`Global`](../enums/codearts_plugin_.TaskScope.md#global) \| [`Workspace`](../enums/codearts_plugin_.TaskScope.md#workspace) |  |
| `name` | `string` |  |
| `source` | `string` |  |
| `execution?` | [`ProcessExecution`](codearts_plugin_.ProcessExecution.md) \| [`ShellExecution`](codearts_plugin_.ShellExecution.md) \| [`CustomExecution`](codearts_plugin_.CustomExecution.md) |  |
| `problemMatchers?` | `string` \| `string`[] |  |

#### Defined in

[index.d.ts:7501](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L7501)

• **new Task**(`taskDefinition`, `name`, `source`, `execution?`, `problemMatchers?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskDefinition` | [`TaskDefinition`](../interfaces/codearts_plugin_.TaskDefinition.md) |  |
| `name` | `string` |  |
| `source` | `string` |  |
| `execution?` | [`ProcessExecution`](codearts_plugin_.ProcessExecution.md) \| [`ShellExecution`](codearts_plugin_.ShellExecution.md) |  |
| `problemMatchers?` | `string` \| `string`[] |  |

#### Defined in

[index.d.ts:7516](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L7516)

## Properties

### definition

• **definition**: [`TaskDefinition`](../interfaces/codearts_plugin_.TaskDefinition.md)

#### Defined in

[index.d.ts:7521](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L7521)

___

### detail

• `Optional` **detail**: `string`

#### Defined in

[index.d.ts:7538](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L7538)

___

### execution

• `Optional` **execution**: [`ProcessExecution`](codearts_plugin_.ProcessExecution.md) \| [`ShellExecution`](codearts_plugin_.ShellExecution.md) \| [`CustomExecution`](codearts_plugin_.CustomExecution.md)

#### Defined in

[index.d.ts:7543](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L7543)

___

### group

• `Optional` **group**: [`TaskGroup`](codearts_plugin_.TaskGroup.md)

#### Defined in

[index.d.ts:7562](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L7562)

___

### isBackground

• **isBackground**: `boolean`

#### Defined in

[index.d.ts:7548](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L7548)

___

### name

• **name**: `string`

#### Defined in

[index.d.ts:7531](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L7531)

___

### presentationOptions

• **presentationOptions**: [`TaskPresentationOptions`](../interfaces/codearts_plugin_.TaskPresentationOptions.md)

#### Defined in

[index.d.ts:7567](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L7567)

___

### problemMatchers

• **problemMatchers**: `string`[]

#### Defined in

[index.d.ts:7573](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L7573)

___

### runOptions

• **runOptions**: [`RunOptions`](../interfaces/codearts_plugin_.RunOptions.md)

#### Defined in

[index.d.ts:7578](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L7578)

___

### scope

• `Readonly` **scope**: `undefined` \| [`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) \| [`Global`](../enums/codearts_plugin_.TaskScope.md#global) \| [`Workspace`](../enums/codearts_plugin_.TaskScope.md#workspace)

#### Defined in

[index.d.ts:7526](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L7526)

___

### source

• **source**: `string`

#### Defined in

[index.d.ts:7554](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L7554)
