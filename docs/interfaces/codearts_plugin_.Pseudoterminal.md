[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / Pseudoterminal

# Interface: Pseudoterminal

["@codearts/plugin"](../modules/_codearts_plugin_.md).Pseudoterminal

Defines the interface of a terminal pty, enabling extensions to control a terminal.

## Table of contents

### Properties

- [onDidChangeName](codearts_plugin_.Pseudoterminal.md#ondidchangename)
- [onDidClose](codearts_plugin_.Pseudoterminal.md#ondidclose)
- [onDidOverrideDimensions](codearts_plugin_.Pseudoterminal.md#ondidoverridedimensions)
- [onDidWrite](codearts_plugin_.Pseudoterminal.md#ondidwrite)

### Methods

- [close](codearts_plugin_.Pseudoterminal.md#close)
- [handleInput](codearts_plugin_.Pseudoterminal.md#handleinput)
- [open](codearts_plugin_.Pseudoterminal.md#open)
- [setDimensions](codearts_plugin_.Pseudoterminal.md#setdimensions)

## Properties

### onDidChangeName

• `Optional` **onDidChangeName**: [`Event`](codearts_plugin_.Event.md)<`string`\>

An event that when fired allows changing the name of the terminal.

Events fired before [open](codearts_plugin_.Pseudoterminal.md#open) is called will be be ignored.

**Example:** Change the terminal name to "My new terminal".
```typescript
const writeEmitter = new vscode.EventEmitter<string>();
const changeNameEmitter = new vscode.EventEmitter<string>();
const pty: vscode.Pseudoterminal = {
  onDidWrite: writeEmitter.event,
  onDidChangeName: changeNameEmitter.event,
  open: () => changeNameEmitter.fire('My new terminal'),
  close: () => {}
};
vscode.window.createTerminal({ name: 'My terminal', pty });
```

#### Defined in

[index.d.ts:11075](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11075)

___

### onDidClose

• `Optional` **onDidClose**: [`Event`](codearts_plugin_.Event.md)<`number` \| `void`\>

An event that when fired will signal that the pty is closed and dispose of the terminal.

Events fired before [open](codearts_plugin_.Pseudoterminal.md#open) is called will be be ignored.

A number can be used to provide an exit code for the terminal. Exit codes must be
positive and a non-zero exit codes signals failure which shows a notification for a
regular terminal and allows dependent tasks to proceed when used with the
`CustomExecution` API.

**Example:** Exit the terminal when "y" is pressed, otherwise show a notification.
```typescript
const writeEmitter = new vscode.EventEmitter<string>();
const closeEmitter = new vscode.EventEmitter<vscode.TerminalDimensions>();
const pty: vscode.Pseudoterminal = {
  onDidWrite: writeEmitter.event,
  onDidClose: closeEmitter.event,
  open: () => writeEmitter.fire('Press y to exit successfully'),
  close: () => {},
  handleInput: data => {
    if (data !== 'y') {
      vscode.window.showInformationMessage('Something went wrong');
    }
    closeEmitter.fire();
  }
};
vscode.window.createTerminal({ name: 'Exit example', pty });
```

#### Defined in

[index.d.ts:11055](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11055)

___

### onDidOverrideDimensions

• `Optional` **onDidOverrideDimensions**: [`Event`](codearts_plugin_.Event.md)<`undefined` \| [`TerminalDimensions`](codearts_plugin_.TerminalDimensions.md)\>

An event that when fired allows overriding the [dimensions](codearts_plugin_.Pseudoterminal.md#setdimensions) of the
terminal. Note that when set, the overridden dimensions will only take effect when they
are lower than the actual dimensions of the terminal (ie. there will never be a scroll
bar). Set to `undefined` for the terminal to go back to the regular dimensions (fit to
the size of the panel).

Events fired before [open](codearts_plugin_.Pseudoterminal.md#open) is called will be be ignored.

**Example:** Override the dimensions of a terminal to 20 columns and 10 rows
```typescript
const dimensionsEmitter = new vscode.EventEmitter<vscode.TerminalDimensions>();
const pty: vscode.Pseudoterminal = {
  onDidWrite: writeEmitter.event,
  onDidOverrideDimensions: dimensionsEmitter.event,
  open: () => {
    dimensionsEmitter.fire({
      columns: 20,
      rows: 10
    });
  },
  close: () => {}
};
vscode.window.createTerminal({ name: 'My terminal', pty });
```

#### Defined in

[index.d.ts:11024](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11024)

___

### onDidWrite

• **onDidWrite**: [`Event`](codearts_plugin_.Event.md)<`string`\>

An event that when fired will write data to the terminal. Unlike
[sendText](codearts_plugin_.Terminal.md#sendtext) which sends text to the underlying child
pseudo-device (the child), this will write the text to parent pseudo-device (the
_terminal_ itself).

Note writing `\n` will just move the cursor down 1 row, you need to write `\r` as well
to move the cursor to the left-most cell.

Events fired before [open](codearts_plugin_.Pseudoterminal.md#open) is called will be be ignored.

**Example:** Write red text to the terminal
```typescript
const writeEmitter = new vscode.EventEmitter<string>();
const pty: vscode.Pseudoterminal = {
  onDidWrite: writeEmitter.event,
  open: () => writeEmitter.fire('\x1b[31mHello world\x1b[0m'),
  close: () => {}
};
vscode.window.createTerminal({ name: 'My terminal', pty });
```

**Example:** Move the cursor to the 10th row and 20th column and write an asterisk
```typescript
writeEmitter.fire('\x1b[10;20H*');
```

#### Defined in

[index.d.ts:10996](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L10996)

## Methods

### close

▸ **close**(): `void`

Implement to handle when the terminal is closed by an act of the user.

#### Returns

`void`

#### Defined in

[index.d.ts:11088](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11088)

___

### handleInput

▸ `Optional` **handleInput**(`data`): `void`

Implement to handle incoming keystrokes in the terminal or when an extension calls
[sendText](codearts_plugin_.Terminal.md#sendtext). `data` contains the keystrokes/text serialized into
their corresponding VT sequence representation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `string` | The incoming data.  **Example:** Echo input in the terminal. The sequence for enter (`\r`) is translated to CRLF to go to a new line and move the cursor to the start of the line. ```typescript const writeEmitter = new vscode.EventEmitter<string>(); const pty: vscode.Pseudoterminal = {   onDidWrite: writeEmitter.event,   open: () => {},   close: () => {},   handleInput: data => writeEmitter.fire(data === '\r' ? '\r\n' : data) }; vscode.window.createTerminal({ name: 'Local echo', pty }); ``` |

#### Returns

`void`

#### Defined in

[index.d.ts:11110](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11110)

___

### open

▸ **open**(`initialDimensions`): `void`

Implement to handle when the pty is open and ready to start firing events.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `initialDimensions` | `undefined` \| [`TerminalDimensions`](codearts_plugin_.TerminalDimensions.md) | The dimensions of the terminal, this will be undefined if the terminal panel has not been opened before this is called. |

#### Returns

`void`

#### Defined in

[index.d.ts:11083](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11083)

___

### setDimensions

▸ `Optional` **setDimensions**(`dimensions`): `void`

Implement to handle when the number of rows and columns that fit into the terminal panel
changes, for example when font size changes or when the panel is resized. The initial
state of a terminal's dimensions should be treated as `undefined` until this is triggered
as the size of a terminal isn't known until it shows up in the user interface.

When dimensions are overridden by
[onDidOverrideDimensions](codearts_plugin_.Pseudoterminal.md#ondidoverridedimensions), `setDimensions` will
continue to be called with the regular panel dimensions, allowing the extension continue
to react dimension changes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dimensions` | [`TerminalDimensions`](codearts_plugin_.TerminalDimensions.md) | The new dimensions. |

#### Returns

`void`

#### Defined in

[index.d.ts:11125](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11125)
