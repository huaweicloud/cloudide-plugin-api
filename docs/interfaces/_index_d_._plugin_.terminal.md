**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Terminal

# Interface: Terminal

An individual terminal instance within the integrated terminal.

## Hierarchy

* **Terminal**

## Index

### Properties

* [creationOptions](_index_d_._plugin_.terminal.md#creationoptions)
* [exitStatus](_index_d_._plugin_.terminal.md#exitstatus)
* [name](_index_d_._plugin_.terminal.md#name)
* [processId](_index_d_._plugin_.terminal.md#processid)

### Methods

* [dispose](_index_d_._plugin_.terminal.md#dispose)
* [hide](_index_d_._plugin_.terminal.md#hide)
* [sendText](_index_d_._plugin_.terminal.md#sendtext)
* [show](_index_d_._plugin_.terminal.md#show)

## Properties

### creationOptions

• `Readonly` **creationOptions**: Readonly\<[TerminalOptions](_index_d_._plugin_.terminaloptions.md) \| [ExtensionTerminalOptions](_index_d_._plugin_.extensionterminaloptions.md)>

*Defined in [index.d.ts:5306](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5306)*

The object used to initialize the terminal, this is useful for example to detecting the
shell type of when the terminal was not launched by this extension or for detecting what
folder the shell was launched in.

___

### exitStatus

• `Readonly` **exitStatus**: [TerminalExitStatus](_index_d_._plugin_.terminalexitstatus.md) \| undefined

*Defined in [index.d.ts:5321](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5321)*

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

___

### name

• `Readonly` **name**: string

*Defined in [index.d.ts:5294](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5294)*

The name of the terminal.

___

### processId

• `Readonly` **processId**: [Thenable](_index_d_.thenable.md)\<number \| undefined>

*Defined in [index.d.ts:5299](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5299)*

The process ID of the shell process.

## Methods

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:5349](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5349)*

Dispose and free associated resources.

**Returns:** void

___

### hide

▸ **hide**(): void

*Defined in [index.d.ts:5344](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5344)*

Hide the terminal panel if this terminal is currently showing.

**Returns:** void

___

### sendText

▸ **sendText**(`text`: string, `addNewLine?`: boolean): void

*Defined in [index.d.ts:5332](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5332)*

Send text to the terminal. The text is written to the stdin of the underlying pty process
(shell) of the terminal.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`text` | string | The text to send. |
`addNewLine?` | boolean | Whether to add a new line to the text being sent, this is normally required to run a command in the terminal. The character(s) added are \n or \r\n depending on the platform. This defaults to `true`.  |

**Returns:** void

___

### show

▸ **show**(`preserveFocus?`: boolean): void

*Defined in [index.d.ts:5339](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5339)*

Show the terminal panel and reveal this terminal in the UI.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`preserveFocus?` | boolean | When `true` the terminal will not take focus.  |

**Returns:** void
