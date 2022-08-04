[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugSession

# Interface: DebugSession

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugSession

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

#### Defined in

[index.d.ts:14120](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14120)

___

### id

• `Readonly` **id**: `string`

#### Defined in

[index.d.ts:14090](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14090)

___

### name

• **name**: `string`

#### Defined in

[index.d.ts:14107](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14107)

___

### parentSession

• `Optional` `Readonly` **parentSession**: [`DebugSession`](codearts_plugin_.DebugSession.md)

#### Defined in

[index.d.ts:14101](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14101)

___

### type

• `Readonly` **type**: `string`

#### Defined in

[index.d.ts:14095](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14095)

___

### workspaceFolder

• `Readonly` **workspaceFolder**: `undefined` \| [`WorkspaceFolder`](codearts_plugin_.WorkspaceFolder.md)

#### Defined in

[index.d.ts:14112](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14112)

## Methods

### customRequest

▸ **customRequest**(`command`, `args?`): [`Thenable`](Thenable.md)<`any`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `command` | `string` |
| `args?` | `any` |

#### Returns

[`Thenable`](Thenable.md)<`any`\>

#### Defined in

[index.d.ts:14125](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14125)

___

### getDebugProtocolBreakpoint

▸ **getDebugProtocolBreakpoint**(`breakpoint`): [`Thenable`](Thenable.md)<`undefined` \| [`DebugProtocolBreakpoint`](codearts_plugin_.DebugProtocolBreakpoint.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `breakpoint` | [`Breakpoint`](../classes/codearts_plugin_.Breakpoint.md) |  |

#### Returns

[`Thenable`](Thenable.md)<`undefined` \| [`DebugProtocolBreakpoint`](codearts_plugin_.DebugProtocolBreakpoint.md)\>

#### Defined in

[index.d.ts:14134](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14134)
