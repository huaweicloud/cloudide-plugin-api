[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DebugSession

# Interface: DebugSession

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DebugSession

A debug session.

## Table of contents

### Properties

- [configuration](cloudide_plugin_.DebugSession.md#configuration)
- [id](cloudide_plugin_.DebugSession.md#id)
- [name](cloudide_plugin_.DebugSession.md#name)
- [type](cloudide_plugin_.DebugSession.md#type)

### Methods

- [customRequest](cloudide_plugin_.DebugSession.md#customrequest)

## Properties

### configuration

• `Readonly` **configuration**: [`DebugConfiguration`](cloudide_plugin_.DebugConfiguration.md)

The "resolved" [debug configuration](#DebugConfiguration) of this session.

#### Defined in

[index.d.ts:9617](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9617)

___

### id

• `Readonly` **id**: `string`

The unique ID of this debug session.

#### Defined in

[index.d.ts:9602](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9602)

___

### name

• `Readonly` **name**: `string`

The debug session's name from the [debug configuration](#DebugConfiguration).

#### Defined in

[index.d.ts:9612](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9612)

___

### type

• `Readonly` **type**: `string`

The debug session's type from the [debug configuration](#DebugConfiguration).

#### Defined in

[index.d.ts:9607](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9607)

## Methods

### customRequest

▸ **customRequest**(`command`, `args?`): `PromiseLike`<`any`\>

Send a custom request to the debug adapter.

#### Parameters

| Name | Type |
| :------ | :------ |
| `command` | `string` |
| `args?` | `any` |

#### Returns

`PromiseLike`<`any`\>

#### Defined in

[index.d.ts:9622](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9622)
