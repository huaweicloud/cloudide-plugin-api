**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Task

# Class: Task

A task to execute

## Hierarchy

* **Task**

## Index

### Constructors

* [constructor](_index_d_._plugin_.task.md#constructor)

### Properties

* [definition](_index_d_._plugin_.task.md#definition)
* [execution](_index_d_._plugin_.task.md#execution)
* [group](_index_d_._plugin_.task.md#group)
* [isBackground](_index_d_._plugin_.task.md#isbackground)
* [name](_index_d_._plugin_.task.md#name)
* [presentationOptions](_index_d_._plugin_.task.md#presentationoptions)
* [problemMatchers](_index_d_._plugin_.task.md#problemmatchers)
* [runOptions](_index_d_._plugin_.task.md#runoptions)
* [scope](_index_d_._plugin_.task.md#scope)
* [source](_index_d_._plugin_.task.md#source)

## Constructors

### constructor

\+ **new Task**(`taskDefinition`: [TaskDefinition](../interfaces/_index_d_._plugin_.taskdefinition.md), `scope`: [WorkspaceFolder](../interfaces/_index_d_._plugin_.workspacefolder.md) \| [Global](../enums/_index_d_._plugin_.taskscope.md#global) \| [Workspace](../enums/_index_d_._plugin_.taskscope.md#workspace), `name`: string, `source`: string, `execution?`: [ProcessExecution](_index_d_._plugin_.processexecution.md) \| [ShellExecution](_index_d_._plugin_.shellexecution.md) \| [CustomExecution](_index_d_._plugin_.customexecution.md), `problemMatchers?`: string \| string[]): [Task](_index_d_._plugin_.task.md)

*Defined in [index.d.ts:5950](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5950)*

Creates a new task.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`taskDefinition` | [TaskDefinition](../interfaces/_index_d_._plugin_.taskdefinition.md) | - |
`scope` | [WorkspaceFolder](../interfaces/_index_d_._plugin_.workspacefolder.md) \| [Global](../enums/_index_d_._plugin_.taskscope.md#global) \| [Workspace](../enums/_index_d_._plugin_.taskscope.md#workspace) | Specifies the task's scope. It is either a global or a workspace task or a task for a specific workspace folder. Global tasks are currently not supported. |
`name` | string | The task's name. Is presented in the user interface. |
`source` | string | The task's source (e.g. 'gulp', 'npm', ...). Is presented in the user interface. |
`execution?` | [ProcessExecution](_index_d_._plugin_.processexecution.md) \| [ShellExecution](_index_d_._plugin_.shellexecution.md) \| [CustomExecution](_index_d_._plugin_.customexecution.md) | The process or shell execution. |
`problemMatchers?` | string \| string[] | the names of problem matchers to use, like '$tsc'  or '$eslint'. Problem matchers can be contributed by an extension using  the `problemMatchers` extension point.  |

**Returns:** [Task](_index_d_._plugin_.task.md)

\+ **new Task**(`taskDefinition`: [TaskDefinition](../interfaces/_index_d_._plugin_.taskdefinition.md), `name`: string, `source`: string, `execution?`: [ProcessExecution](_index_d_._plugin_.processexecution.md) \| [ShellExecution](_index_d_._plugin_.shellexecution.md), `problemMatchers?`: string \| string[]): [Task](_index_d_._plugin_.task.md)

*Defined in [index.d.ts:5964](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5964)*

~~Creates a new task.~~

**`deprecated`** Use the new constructors that allow specifying a scope for the task.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`taskDefinition` | [TaskDefinition](../interfaces/_index_d_._plugin_.taskdefinition.md) | - |
`name` | string | The task's name. Is presented in the user interface. |
`source` | string | The task's source (e.g. 'gulp', 'npm', ...). Is presented in the user interface. |
`execution?` | [ProcessExecution](_index_d_._plugin_.processexecution.md) \| [ShellExecution](_index_d_._plugin_.shellexecution.md) | The process or shell execution. |
`problemMatchers?` | string \| string[] | the names of problem matchers to use, like '$tsc'  or '$eslint'. Problem matchers can be contributed by an extension using  the `problemMatchers` extension point.  |

**Returns:** [Task](_index_d_._plugin_.task.md)

## Properties

### definition

•  **definition**: [TaskDefinition](../interfaces/_index_d_._plugin_.taskdefinition.md)

*Defined in [index.d.ts:5984](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5984)*

The task's definition.

___

### execution

• `Optional` **execution**: [ProcessExecution](_index_d_._plugin_.processexecution.md) \| [ShellExecution](_index_d_._plugin_.shellexecution.md) \| [CustomExecution](_index_d_._plugin_.customexecution.md)

*Defined in [index.d.ts:5999](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5999)*

The task's execution engine

___

### group

• `Optional` **group**: [TaskGroup](_index_d_._plugin_.taskgroup.md)

*Defined in [index.d.ts:6018](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6018)*

The task group this tasks belongs to. See TaskGroup
for a predefined set of available groups.
Defaults to undefined meaning that the task doesn't
belong to any special group.

___

### isBackground

•  **isBackground**: boolean

*Defined in [index.d.ts:6004](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6004)*

Whether the task is a background task or not.

___

### name

•  **name**: string

*Defined in [index.d.ts:5994](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5994)*

The task's name

___

### presentationOptions

•  **presentationOptions**: [TaskPresentationOptions](../interfaces/_index_d_._plugin_.taskpresentationoptions.md)

*Defined in [index.d.ts:6023](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6023)*

The presentation options. Defaults to an empty literal.

___

### problemMatchers

•  **problemMatchers**: string[]

*Defined in [index.d.ts:6029](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6029)*

The problem matchers attached to the task. Defaults to an empty
array.

___

### runOptions

•  **runOptions**: [RunOptions](../interfaces/_index_d_._plugin_.runoptions.md)

*Defined in [index.d.ts:6034](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6034)*

Run options for the task

___

### scope

• `Optional` `Readonly` **scope**: [Global](../enums/_index_d_._plugin_.taskscope.md#global) \| [Workspace](../enums/_index_d_._plugin_.taskscope.md#workspace) \| [WorkspaceFolder](../interfaces/_index_d_._plugin_.workspacefolder.md)

*Defined in [index.d.ts:5989](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5989)*

The task's scope.

___

### source

•  **source**: string

*Defined in [index.d.ts:6010](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L6010)*

A human-readable string describing the source of this shell task, e.g. 'gulp'
or 'npm'. Supports rendering of [theme icons](#ThemeIcon) via the `$(<name>)`-syntax.
