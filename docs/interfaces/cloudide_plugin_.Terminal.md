[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Terminal

# Interface: Terminal

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Terminal

Definition of the terminal emulator.

## Table of contents

### Properties

- [name](cloudide_plugin_.Terminal.md#name)
- [processId](cloudide_plugin_.Terminal.md#processid)

### Methods

- [dispose](cloudide_plugin_.Terminal.md#dispose)
- [hide](cloudide_plugin_.Terminal.md#hide)
- [sendText](cloudide_plugin_.Terminal.md#sendtext)
- [show](cloudide_plugin_.Terminal.md#show)

## Properties

### name

• `Readonly` **name**: `string`

Human readable representation of the terminal in the UI.

#### Defined in

[index.d.ts:2746](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2746)

___

### processId

• `Readonly` **processId**: `PromiseLike`<`number`\>

Terminal id.

#### Defined in

[index.d.ts:2751](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2751)

## Methods

### dispose

▸ **dispose**(): `void`

Destroy terminal.

#### Returns

`void`

#### Defined in

[index.d.ts:2774](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2774)

___

### hide

▸ **hide**(): `void`

Hide terminal panel.

#### Returns

`void`

#### Defined in

[index.d.ts:2769](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2769)

___

### sendText

▸ **sendText**(`text`, `addNewLine?`): `void`

Send text to the terminal.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | text content. |
| `addNewLine?` | `boolean` | in case true - apply new line after the text, otherwise don't apply new line. This defaults to `true`. |

#### Returns

`void`

#### Defined in

[index.d.ts:2758](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2758)

___

### show

▸ **show**(`preserveFocus?`): `void`

Show created terminal on the UI.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `preserveFocus?` | `boolean` | in case true - set up focus on the terminal widget, otherwise show terminal without focus. |

#### Returns

`void`

#### Defined in

[index.d.ts:2764](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2764)
