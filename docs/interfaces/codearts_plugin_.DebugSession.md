[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugSession

# Interface: DebugSession

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugSession

A debug session.

## Table of contents

### Properties

- [configuration](codearts_plugin_.DebugSession.md#configuration)
- [id](codearts_plugin_.DebugSession.md#id)
- [name](codearts_plugin_.DebugSession.md#name)
- [parentSession](codearts_plugin_.DebugSession.md#parentsession)
- [type](codearts_plugin_.DebugSession.md#type)
- [workspaceFolder](codearts_plugin_.DebugSession.md#workspacefolder)

### Methods

- [customRequest](codearts_plugin_.DebugSession.md#customrequest)
- [getDebugProtocolBreakpoint](codearts_plugin_.DebugSession.md#getdebugprotocolbreakpoint)

## Properties

### configuration

• `Readonly` **configuration**: [`DebugConfiguration`](codearts_plugin_.DebugConfiguration.md)

The "resolved" [debug configuration](codearts_plugin_.DebugConfiguration.md) of this session.
"Resolved" means that
- all variables have been substituted and
- platform specific attribute sections have been "flattened" for the matching platform and removed for non-matching platforms.

#### Defined in

[index.d.ts:14957](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14957)

___

### id

• `Readonly` **id**: `string`

The unique ID of this debug session.

#### Defined in

[index.d.ts:14927](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14927)

___

### name

• **name**: `string`

The debug session's name is initially taken from the [debug configuration](codearts_plugin_.DebugConfiguration.md).
Any changes will be properly reflected in the UI.

#### Defined in

[index.d.ts:14944](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14944)

___

### parentSession

• `Optional` `Readonly` **parentSession**: [`DebugSession`](codearts_plugin_.DebugSession.md)

The parent session of this debug session, if it was created as a child.

**`See`**

DebugSessionOptions.parentSession

#### Defined in

[index.d.ts:14938](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14938)

___

### type

• `Readonly` **type**: `string`

The debug session's type from the [debug configuration](codearts_plugin_.DebugConfiguration.md).

#### Defined in

[index.d.ts:14932](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14932)

___

### workspaceFolder

• `Readonly` **workspaceFolder**: `undefined` \| [`WorkspaceFolder`](codearts_plugin_.WorkspaceFolder.md)

The workspace folder of this session or `undefined` for a folderless setup.

#### Defined in

[index.d.ts:14949](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14949)

## Methods

### customRequest

▸ **customRequest**(`command`, `args?`): [`Thenable`](Thenable.md)<`any`\>

Send a custom request to the debug adapter.

#### Parameters

| Name | Type |
| :------ | :------ |
| `command` | `string` |
| `args?` | `any` |

#### Returns

[`Thenable`](Thenable.md)<`any`\>

#### Defined in

[index.d.ts:14962](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14962)

___

### getDebugProtocolBreakpoint

▸ **getDebugProtocolBreakpoint**(`breakpoint`): [`Thenable`](Thenable.md)<`undefined` \| [`DebugProtocolBreakpoint`](codearts_plugin_.DebugProtocolBreakpoint.md)\>

Maps a breakpoint in the editor to the corresponding Debug Adapter Protocol (DAP) breakpoint that is managed by the debug adapter of the debug session.
If no DAP breakpoint exists (either because the editor breakpoint was not yet registered or because the debug adapter is not interested in the breakpoint), the value `undefined` is returned.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `breakpoint` | [`Breakpoint`](../classes/codearts_plugin_.Breakpoint.md) | A [Breakpoint](../classes/codearts_plugin_.Breakpoint.md) in the editor. |

#### Returns

[`Thenable`](Thenable.md)<`undefined` \| [`DebugProtocolBreakpoint`](codearts_plugin_.DebugProtocolBreakpoint.md)\>

A promise that resolves to the Debug Adapter Protocol breakpoint or `undefined`.

#### Defined in

[index.d.ts:14971](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14971)
