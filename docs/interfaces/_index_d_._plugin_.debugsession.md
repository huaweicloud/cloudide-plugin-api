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
* [getDebugProtocolBreakpoint](_index_d_._plugin_.debugsession.md#getdebugprotocolbreakpoint)

## Properties

### configuration

• `Readonly` **configuration**: [DebugConfiguration](_index_d_._plugin_.debugconfiguration.md)

*Defined in [index.d.ts:11540](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11540)*

The "resolved" [debug configuration](#DebugConfiguration) of this session.
"Resolved" means that
- all variables have been substituted and
- platform specific attribute sections have been "flattened" for the matching platform and removed for non-matching platforms.

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:11516](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11516)*

The unique ID of this debug session.

___

### name

•  **name**: string

*Defined in [index.d.ts:11527](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11527)*

The debug session's name is initially taken from the [debug configuration](#DebugConfiguration).
Any changes will be properly reflected in the UI.

___

### type

• `Readonly` **type**: string

*Defined in [index.d.ts:11521](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11521)*

The debug session's type from the [debug configuration](#DebugConfiguration).

___

### workspaceFolder

• `Readonly` **workspaceFolder**: [WorkspaceFolder](_index_d_._plugin_.workspacefolder.md) \| undefined

*Defined in [index.d.ts:11532](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11532)*

The workspace folder of this session or `undefined` for a folderless setup.

## Methods

### customRequest

▸ **customRequest**(`command`: string, `args?`: any): [Thenable](_index_d_.thenable.md)\<any>

*Defined in [index.d.ts:11545](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11545)*

Send a custom request to the debug adapter.

#### Parameters:

Name | Type |
------ | ------ |
`command` | string |
`args?` | any |

**Returns:** [Thenable](_index_d_.thenable.md)\<any>

___

### getDebugProtocolBreakpoint

▸ **getDebugProtocolBreakpoint**(`breakpoint`: [Breakpoint](../classes/_index_d_._plugin_.breakpoint.md)): [Thenable](_index_d_.thenable.md)\<[DebugProtocolBreakpoint](_index_d_._plugin_.debugprotocolbreakpoint.md) \| undefined>

*Defined in [index.d.ts:11554](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11554)*

Maps a VS Code breakpoint to the corresponding Debug Adapter Protocol (DAP) breakpoint that is managed by the debug adapter of the debug session.
If no DAP breakpoint exists (either because the VS Code breakpoint was not yet registered or because the debug adapter is not interested in the breakpoint), the value `undefined` is returned.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`breakpoint` | [Breakpoint](../classes/_index_d_._plugin_.breakpoint.md) | A VS Code [breakpoint](#Breakpoint). |

**Returns:** [Thenable](_index_d_.thenable.md)\<[DebugProtocolBreakpoint](_index_d_._plugin_.debugprotocolbreakpoint.md) \| undefined>

A promise that resolves to the Debug Adapter Protocol breakpoint or `undefined`.
