[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Terminal

# Interface: Terminal

["@codearts/plugin"](../modules/_codearts_plugin_.md).Terminal

An individual terminal instance within the integrated terminal.

## Table of contents

### Properties

- [creationOptions](codearts_plugin_.Terminal.md#creationoptions)
- [exitStatus](codearts_plugin_.Terminal.md#exitstatus)
- [id](codearts_plugin_.Terminal.md#id)
- [name](codearts_plugin_.Terminal.md#name)
- [processId](codearts_plugin_.Terminal.md#processid)
- [state](codearts_plugin_.Terminal.md#state)

### Methods

- [dispose](codearts_plugin_.Terminal.md#dispose)
- [hide](codearts_plugin_.Terminal.md#hide)
- [sendText](codearts_plugin_.Terminal.md#sendtext)
- [setColor](codearts_plugin_.Terminal.md#setcolor)
- [show](codearts_plugin_.Terminal.md#show)

## Properties

### creationOptions

• `Readonly` **creationOptions**: `Readonly`<[`TerminalOptions`](codearts_plugin_.TerminalOptions.md) \| [`ExtensionTerminalOptions`](codearts_plugin_.ExtensionTerminalOptions.md)\>

The object used to initialize the terminal, this is useful for example to detecting the
shell type of when the terminal was not launched by this extension or for detecting what
folder the shell was launched in.

#### Defined in

[index.d.ts:6482](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L6482)

___

### exitStatus

• `Readonly` **exitStatus**: `undefined` \| [`TerminalExitStatus`](codearts_plugin_.TerminalExitStatus.md)

The exit status of the terminal, this will be undefined while the terminal is active.

**Example:** Show a notification with the exit code when the terminal exits with a
non-zero exit code.
```typescript
window.onDidCloseTerminal(t => {
  if (t.exitStatus && t.exitStatus.code) {
  	vscode.window.showInformationMessage(`Exit code: ${t.exitStatus.code}`);
  }
});
```

#### Defined in

[index.d.ts:6497](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L6497)

___

### id

• `Readonly` **id**: [`Thenable`](Thenable.md)<`string`\>

The unique id of the terminal.

#### Defined in

[index.d.ts:6465](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L6465)

___

### name

• `Readonly` **name**: `string`

The name of the terminal.

#### Defined in

[index.d.ts:6470](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L6470)

___

### processId

• `Readonly` **processId**: [`Thenable`](Thenable.md)<`undefined` \| `number`\>

The process ID of the shell process.

#### Defined in

[index.d.ts:6475](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L6475)

___

### state

• `Readonly` **state**: [`TerminalState`](codearts_plugin_.TerminalState.md)

The current state of the [Terminal](codearts_plugin_.Terminal.md).

#### Defined in

[index.d.ts:6502](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L6502)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose and free associated resources.

#### Returns

`void`

#### Defined in

[index.d.ts:6536](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L6536)

___

### hide

▸ **hide**(): `void`

Hide the terminal panel if this terminal is currently showing.

#### Returns

`void`

#### Defined in

[index.d.ts:6531](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L6531)

___

### sendText

▸ **sendText**(`text`, `addNewLine?`): `void`

Send text to the terminal. The text is written to the stdin of the underlying pty process
(shell) of the terminal.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | The text to send. |
| `addNewLine?` | `boolean` | Whether to add a new line to the text being sent, this is normally required to run a command in the terminal. The character(s) added are \n or \r\n depending on the platform. This defaults to `true`. |

#### Returns

`void`

#### Defined in

[index.d.ts:6513](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L6513)

___

### setColor

▸ **setColor**(`colorId`): `void`

Change the color of the terminal icon.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `colorId` | [`TerminalAnsiColorId`](../enums/codearts_plugin_.TerminalAnsiColorId.md) | Terminal Icon Color Enumeration |

#### Returns

`void`

#### Defined in

[index.d.ts:6519](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L6519)

___

### show

▸ **show**(`preserveFocus?`): `void`

Show the terminal panel and reveal this terminal in the UI.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `preserveFocus?` | `boolean` | When `true` the terminal will not take focus. |

#### Returns

`void`

#### Defined in

[index.d.ts:6526](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L6526)
