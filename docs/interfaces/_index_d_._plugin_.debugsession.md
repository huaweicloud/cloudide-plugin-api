**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugSession

# Interface: DebugSession

A debug session.

## Hierarchy

* **DebugSession**

## Index

### Properties

* [configuration](_index_d_._plugin_.debugsession.md#configuration)
* [id](_index_d_._plugin_.debugsession.md#id)
* [name](_index_d_._plugin_.debugsession.md#name)
* [type](_index_d_._plugin_.debugsession.md#type)
* [workspaceFolder](_index_d_._plugin_.debugsession.md#workspacefolder)

### Methods

* [customRequest](_index_d_._plugin_.debugsession.md#customrequest)

## Properties

### configuration

• `Readonly` **configuration**: [DebugConfiguration](_index_d_._plugin_.debugconfiguration.md)

*Defined in [index.d.ts:10141](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10141)*

The "resolved" [debug configuration](#DebugConfiguration) of this session.
"Resolved" means that
- all variables have been substituted and
- platform specific attribute sections have been "flattened" for the matching platform and removed for non-matching platforms.

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:10117](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10117)*

The unique ID of this debug session.

___

### name

•  **name**: string

*Defined in [index.d.ts:10128](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10128)*

The debug session's name is initially taken from the [debug configuration](#DebugConfiguration).
Any changes will be properly reflected in the UI.

___

### type

• `Readonly` **type**: string

*Defined in [index.d.ts:10122](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10122)*

The debug session's type from the [debug configuration](#DebugConfiguration).

___

### workspaceFolder

• `Readonly` **workspaceFolder**: [WorkspaceFolder](_index_d_._plugin_.workspacefolder.md) \| undefined

*Defined in [index.d.ts:10133](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10133)*

The workspace folder of this session or `undefined` for a folderless setup.

## Methods

### customRequest

▸ **customRequest**(`command`: string, `args?`: any): [Thenable](_index_d_.thenable.md)\<any>

*Defined in [index.d.ts:10146](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10146)*

Send a custom request to the debug adapter.

#### Parameters:

Name | Type |
------ | ------ |
`command` | string |
`args?` | any |

**Returns:** [Thenable](_index_d_.thenable.md)\<any>
