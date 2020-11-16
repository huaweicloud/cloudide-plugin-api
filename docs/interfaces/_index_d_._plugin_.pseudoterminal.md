**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / Pseudoterminal

# Interface: Pseudoterminal

Defines the interface of a terminal pty, enabling extensions to control a terminal.

## Hierarchy

* **Pseudoterminal**

## Index

### Properties

* [onDidClose](_index_d_._plugin_.pseudoterminal.md#ondidclose)
* [onDidOverrideDimensions](_index_d_._plugin_.pseudoterminal.md#ondidoverridedimensions)
* [onDidWrite](_index_d_._plugin_.pseudoterminal.md#ondidwrite)

### Methods

* [close](_index_d_._plugin_.pseudoterminal.md#close)
* [handleInput](_index_d_._plugin_.pseudoterminal.md#handleinput)
* [open](_index_d_._plugin_.pseudoterminal.md#open)
* [setDimensions](_index_d_._plugin_.pseudoterminal.md#setdimensions)

## Properties

### onDidClose

• `Optional` **onDidClose**: [Event](_index_d_._plugin_.event.md)\<void \| number>

*Defined in [index.d.ts:8218](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8218)*

An event that when fired will signal that the pty is closed and dispose of the terminal.

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

___

### onDidOverrideDimensions

• `Optional` **onDidOverrideDimensions**: [Event](_index_d_._plugin_.event.md)\<[TerminalDimensions](_index_d_._plugin_.terminaldimensions.md) \| undefined>

*Defined in [index.d.ts:8189](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8189)*

An event that when fired allows overriding the [dimensions](#Pseudoterminal.setDimensions) of the
terminal. Note that when set, the overridden dimensions will only take effect when they
are lower than the actual dimensions of the terminal (ie. there will never be a scroll
bar). Set to `undefined` for the terminal to go back to the regular dimensions (fit to
the size of the panel).

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

___

### onDidWrite

•  **onDidWrite**: [Event](_index_d_._plugin_.event.md)\<string>

*Defined in [index.d.ts:8163](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8163)*

An event that when fired will write data to the terminal. Unlike
[Terminal.sendText](#Terminal.sendText) which sends text to the underlying _process_
(the pty "slave"), this will write the text to the terminal itself (the pty "master").

Note writing `\n` will just move the cursor down 1 row, you need to write `\r` as well
to move the cursor to the left-most cell.

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

## Methods

### close

▸ **close**(): void

*Defined in [index.d.ts:8231](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8231)*

Implement to handle when the terminal is closed by an act of the user.

**Returns:** void

___

### handleInput

▸ `Optional`**handleInput**(`data`: string): void

*Defined in [index.d.ts:8253](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8253)*

Implement to handle incoming keystrokes in the terminal or when an extension calls
[Terminal.sendText](#Terminal.sendText). `data` contains the keystrokes/text serialized into
their corresponding VT sequence representation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`data` | string | The incoming data.  **Example:** Echo input in the terminal. The sequence for enter (`\r`) is translated to CRLF to go to a new line and move the cursor to the start of the line. ```typescript const writeEmitter = new vscode.EventEmitter<string>(); const pty: vscode.Pseudoterminal = {   onDidWrite: writeEmitter.event,   open: () => {},   close: () => {},   handleInput: data => writeEmitter.fire(data === '\r' ? '\r\n' : data) }; vscode.window.createTerminal({ name: 'Local echo', pty }); ```  |

**Returns:** void

___

### open

▸ **open**(`initialDimensions`: [TerminalDimensions](_index_d_._plugin_.terminaldimensions.md) \| undefined): void

*Defined in [index.d.ts:8226](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8226)*

Implement to handle when the pty is open and ready to start firing events.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`initialDimensions` | [TerminalDimensions](_index_d_._plugin_.terminaldimensions.md) \| undefined | The dimensions of the terminal, this will be undefined if the terminal panel has not been opened before this is called.  |

**Returns:** void

___

### setDimensions

▸ `Optional`**setDimensions**(`dimensions`: [TerminalDimensions](_index_d_._plugin_.terminaldimensions.md)): void

*Defined in [index.d.ts:8268](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8268)*

Implement to handle when the number of rows and columns that fit into the terminal panel
changes, for example when font size changes or when the panel is resized. The initial
state of a terminal's dimensions should be treated as `undefined` until this is triggered
as the size of a terminal isn't know until it shows up in the user interface.

When dimensions are overridden by
[onDidOverrideDimensions](#Pseudoterminal.onDidOverrideDimensions), `setDimensions` will
continue to be called with the regular panel dimensions, allowing the extension continue
to react dimension changes.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`dimensions` | [TerminalDimensions](_index_d_._plugin_.terminaldimensions.md) | The new dimensions.  |

**Returns:** void
