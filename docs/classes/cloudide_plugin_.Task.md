[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Task

# Class: Task

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Task

## Hierarchy

- **`Task`**

  ↳ [`Task2`](cloudide_plugin_.Task2.md)

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.Task.md#constructor)

### Properties

- [definition](cloudide_plugin_.Task.md#definition)
- [execution](cloudide_plugin_.Task.md#execution)
- [group](cloudide_plugin_.Task.md#group)
- [isBackground](cloudide_plugin_.Task.md#isbackground)
- [name](cloudide_plugin_.Task.md#name)
- [presentationOptions](cloudide_plugin_.Task.md#presentationoptions)
- [problemMatchers](cloudide_plugin_.Task.md#problemmatchers)
- [scope](cloudide_plugin_.Task.md#scope)
- [source](cloudide_plugin_.Task.md#source)

## Constructors

### constructor

• **new Task**(`taskDefinition`, `scope`, `name`, `source?`, `execution?`, `problemMatchers?`)

Creates a new task.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskDefinition` | [`TaskDefinition`](../interfaces/cloudide_plugin_.TaskDefinition.md) | - |
| `scope` | [`WorkspaceFolder`](../interfaces/cloudide_plugin_.WorkspaceFolder.md) \| [`Global`](../enums/cloudide_plugin_.TaskScope.md#global) \| [`Workspace`](../enums/cloudide_plugin_.TaskScope.md#workspace) | Specifies the task's scope. |
| `name` | `string` | The task's name. Is presented in the user interface. |
| `source?` | `string` | The task's source (e.g. 'gulp', 'npm', ...). Is presented in the user interface. |
| `execution?` | [`ShellExecution`](cloudide_plugin_.ShellExecution.md) \| [`ProcessExecution`](cloudide_plugin_.ProcessExecution.md) \| [`CustomExecution`](cloudide_plugin_.CustomExecution.md) | The process, shell or custom execution. |
| `problemMatchers?` | `string` \| `string`[] | the names of problem matchers to use, like '$tsc' or '$eslint'. Problem matchers can be contributed by an extension using the `problemMatchers` extension point. |

#### Defined in

[index.d.ts:10496](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10496)

• **new Task**(`taskDefinition`, `name`, `source`, `execution?`, `problemMatchers?`)

~~Creates a new task.~~

**`Deprecated`**

Use the new constructors that allow specifying a scope for the task.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskDefinition` | [`TaskDefinition`](../interfaces/cloudide_plugin_.TaskDefinition.md) | - |
| `name` | `string` | The task's name. Is presented in the user interface. |
| `source` | `string` | The task's source (e.g. 'gulp', 'npm', ...). Is presented in the user interface. |
| `execution?` | [`ShellExecution`](cloudide_plugin_.ShellExecution.md) \| [`ProcessExecution`](cloudide_plugin_.ProcessExecution.md) \| [`CustomExecution`](cloudide_plugin_.CustomExecution.md) | The process, shell or custom execution. |
| `problemMatchers?` | `string` \| `string`[] | the names of problem matchers to use, like '$tsc' or '$eslint'. Problem matchers can be contributed by an extension using the `problemMatchers` extension point. |

#### Defined in

[index.d.ts:10517](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10517)

## Properties

### definition

• **definition**: [`TaskDefinition`](../interfaces/cloudide_plugin_.TaskDefinition.md)

The task's definition.

#### Defined in

[index.d.ts:10528](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10528)

___

### execution

• `Optional` **execution**: [`ShellExecution`](cloudide_plugin_.ShellExecution.md) \| [`ProcessExecution`](cloudide_plugin_.ProcessExecution.md) \| [`CustomExecution`](cloudide_plugin_.CustomExecution.md)

The task's execution engine

#### Defined in

[index.d.ts:10534](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10534)

___

### group

• `Optional` **group**: [`TaskGroup`](cloudide_plugin_.TaskGroup.md)

The task group this tasks belongs to. See TaskGroup
for a predefined set of available groups.
Defaults to undefined meaning that the task doesn't
belong to any special group.

#### Defined in

[index.d.ts:10551](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10551)

___

### isBackground

• `Optional` **isBackground**: `boolean`

Whether the task is a background task or not.

#### Defined in

[index.d.ts:10537](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10537)

___

### name

• **name**: `string`

The task's name

#### Defined in

[index.d.ts:10525](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10525)

___

### presentationOptions

• `Optional` **presentationOptions**: [`TaskPresentationOptions`](../interfaces/cloudide_plugin_.TaskPresentationOptions.md)

The presentation options. Defaults to an empty literal.

#### Defined in

[index.d.ts:10554](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10554)

___

### problemMatchers

• `Optional` **problemMatchers**: `string`[]

The problem matchers attached to the task. Defaults to an empty
array.

#### Defined in

[index.d.ts:10560](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10560)

___

### scope

• `Optional` **scope**: [`WorkspaceFolder`](../interfaces/cloudide_plugin_.WorkspaceFolder.md) \| [`Global`](../enums/cloudide_plugin_.TaskScope.md#global) \| [`Workspace`](../enums/cloudide_plugin_.TaskScope.md#workspace)

The task's scope.

#### Defined in

[index.d.ts:10531](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10531)

___

### source

• `Optional` **source**: `string`

A human-readable string describing the source of this
shell task, e.g. 'gulp' or 'npm'.

#### Defined in

[index.d.ts:10543](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10543)
