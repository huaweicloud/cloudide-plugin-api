[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Terminal

# Interface: Terminal

["@codearts/plugin"](../modules/_codearts_plugin_.md).Terminal

## Table of contents

### Properties

- [creationOptions](codearts_plugin_.Terminal.md#creationoptions)
- [exitStatus](codearts_plugin_.Terminal.md#exitstatus)
- [name](codearts_plugin_.Terminal.md#name)
- [processId](codearts_plugin_.Terminal.md#processid)
- [state](codearts_plugin_.Terminal.md#state)

### Methods

- [dispose](codearts_plugin_.Terminal.md#dispose)
- [hide](codearts_plugin_.Terminal.md#hide)
- [sendText](codearts_plugin_.Terminal.md#sendtext)
- [show](codearts_plugin_.Terminal.md#show)

## Properties

### creationOptions

• `Readonly` **creationOptions**: `Readonly`<[`TerminalOptions`](codearts_plugin_.TerminalOptions.md) \| [`ExtensionTerminalOptions`](codearts_plugin_.ExtensionTerminalOptions.md)\>

#### Defined in

[index.d.ts:6433](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L6433)

___

### exitStatus

• `Readonly` **exitStatus**: `undefined` \| [`TerminalExitStatus`](codearts_plugin_.TerminalExitStatus.md)

#### Defined in

[index.d.ts:6448](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L6448)

___

### name

• `Readonly` **name**: `string`

#### Defined in

[index.d.ts:6421](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L6421)

___

### processId

• `Readonly` **processId**: [`Thenable`](Thenable.md)<`undefined` \| `number`\>

#### Defined in

[index.d.ts:6426](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L6426)

___

### state

• `Readonly` **state**: [`TerminalState`](codearts_plugin_.TerminalState.md)

#### Defined in

[index.d.ts:6453](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L6453)

## Methods

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:6481](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L6481)

___

### hide

▸ **hide**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:6476](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L6476)

___

### sendText

▸ **sendText**(`text`, `addNewLine?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` |  |
| `addNewLine?` | `boolean` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:6464](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L6464)

___

### show

▸ **show**(`preserveFocus?`): `void`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `preserveFocus?` | `boolean` |  |

#### Returns

`void`

#### Defined in

[index.d.ts:6471](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L6471)
