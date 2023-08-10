[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Task

# Class: Task

["@codearts/plugin"](../modules/_codearts_plugin_.md).Task

A task to execute

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

Creates a new task.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskDefinition` | [`TaskDefinition`](../interfaces/codearts_plugin_.TaskDefinition.md) | The task definition as defined in the taskDefinitions extension point. |
| `scope` | [`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) \| [`Global`](../enums/codearts_plugin_.TaskScope.md#global) \| [`Workspace`](../enums/codearts_plugin_.TaskScope.md#workspace) | Specifies the task's scope. It is either a global or a workspace task or a task for a specific workspace folder. Global tasks are currently not supported. |
| `name` | `string` | The task's name. Is presented in the user interface. |
| `source` | `string` | The task's source (e.g. 'gulp', 'npm', ...). Is presented in the user interface. |
| `execution?` | [`ProcessExecution`](codearts_plugin_.ProcessExecution.md) \| [`ShellExecution`](codearts_plugin_.ShellExecution.md) \| [`CustomExecution`](codearts_plugin_.CustomExecution.md) | The process or shell execution. |
| `problemMatchers?` | `string` \| `string`[] | the names of problem matchers to use, like '$tsc'  or '$eslint'. Problem matchers can be contributed by an extension using  the `problemMatchers` extension point. |

#### Defined in

[index.d.ts:7628](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7628)

• **new Task**(`taskDefinition`, `name`, `source`, `execution?`, `problemMatchers?`)

Creates a new task.

**`Deprecated`**

Use the new constructors that allow specifying a scope for the task.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskDefinition` | [`TaskDefinition`](../interfaces/codearts_plugin_.TaskDefinition.md) | The task definition as defined in the taskDefinitions extension point. |
| `name` | `string` | The task's name. Is presented in the user interface. |
| `source` | `string` | The task's source (e.g. 'gulp', 'npm', ...). Is presented in the user interface. |
| `execution?` | [`ProcessExecution`](codearts_plugin_.ProcessExecution.md) \| [`ShellExecution`](codearts_plugin_.ShellExecution.md) | The process or shell execution. |
| `problemMatchers?` | `string` \| `string`[] | the names of problem matchers to use, like '$tsc'  or '$eslint'. Problem matchers can be contributed by an extension using  the `problemMatchers` extension point. |

#### Defined in

[index.d.ts:7643](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7643)

## Properties

### definition

• **definition**: [`TaskDefinition`](../interfaces/codearts_plugin_.TaskDefinition.md)

The task's definition.

#### Defined in

[index.d.ts:7648](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7648)

___

### detail

• `Optional` **detail**: `string`

A human-readable string which is rendered less prominently on a separate line in places
where the task's name is displayed. Supports rendering of [theme icons](codearts_plugin_.ThemeIcon.md)
via the `$(<name>)`-syntax.

#### Defined in

[index.d.ts:7665](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7665)

___

### execution

• `Optional` **execution**: [`ProcessExecution`](codearts_plugin_.ProcessExecution.md) \| [`ShellExecution`](codearts_plugin_.ShellExecution.md) \| [`CustomExecution`](codearts_plugin_.CustomExecution.md)

The task's execution engine

#### Defined in

[index.d.ts:7670](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7670)

___

### group

• `Optional` **group**: [`TaskGroup`](codearts_plugin_.TaskGroup.md)

The task group this tasks belongs to. See TaskGroup
for a predefined set of available groups.
Defaults to undefined meaning that the task doesn't
belong to any special group.

#### Defined in

[index.d.ts:7689](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7689)

___

### isBackground

• **isBackground**: `boolean`

Whether the task is a background task or not.

#### Defined in

[index.d.ts:7675](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7675)

___

### name

• **name**: `string`

The task's name

#### Defined in

[index.d.ts:7658](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7658)

___

### presentationOptions

• **presentationOptions**: [`TaskPresentationOptions`](../interfaces/codearts_plugin_.TaskPresentationOptions.md)

The presentation options. Defaults to an empty literal.

#### Defined in

[index.d.ts:7694](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7694)

___

### problemMatchers

• **problemMatchers**: `string`[]

The problem matchers attached to the task. Defaults to an empty
array.

#### Defined in

[index.d.ts:7700](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7700)

___

### runOptions

• **runOptions**: [`RunOptions`](../interfaces/codearts_plugin_.RunOptions.md)

Run options for the task

#### Defined in

[index.d.ts:7705](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7705)

___

### scope

• `Readonly` **scope**: `undefined` \| [`WorkspaceFolder`](../interfaces/codearts_plugin_.WorkspaceFolder.md) \| [`Global`](../enums/codearts_plugin_.TaskScope.md#global) \| [`Workspace`](../enums/codearts_plugin_.TaskScope.md#workspace)

The task's scope.

#### Defined in

[index.d.ts:7653](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7653)

___

### source

• **source**: `string`

A human-readable string describing the source of this shell task, e.g. 'gulp'
or 'npm'. Supports rendering of [theme icons](codearts_plugin_.ThemeIcon.md) via the `$(<name>)`-syntax.

#### Defined in

[index.d.ts:7681](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L7681)
