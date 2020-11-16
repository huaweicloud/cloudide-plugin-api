**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](_index_d_.md) / ["plugin"](_index_d_._plugin_.md) / commands

# Namespace: commands

Namespace for dealing with commands. In short, a command is a function with a
unique identifier. The function is sometimes also called _command handler_.

Commands can be added to the editor using the [registerCommand](#commands.registerCommand)
and [registerTextEditorCommand](#commands.registerTextEditorCommand) functions. Commands
can be executed [manually](#commands.executeCommand) or from a UI gesture. Those are:

* palette - Use the `commands`-section in `package.json` to make a command show in
the [command palette](https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette).
* keybinding - Use the `keybindings`-section in `package.json` to enable
[keybindings](https://code.visualstudio.com/docs/getstarted/keybindings#_customizing-shortcuts)
for your extension.

Commands from other extensions and from the editor itself are accessible to an extension. However,
when invoking an editor command not all argument types are supported.

This is a sample that registers a command handler and adds an entry for that command to the palette. First
register a command handler with the identifier `extension.sayHello`.
```javascript
commands.registerCommand('extension.sayHello', () => {
	window.showInformationMessage('Hello World!');
});
```
Second, bind the command identifier to a title under which it will show in the palette (`package.json`).
```json
{
	"contributes": {
		"commands": [{
			"command": "extension.sayHello",
			"title": "Hello World"
		}]
	}
}
```

## Index

### Functions

* [executeCommand](_index_d_._plugin_.commands.md#executecommand)
* [getCommands](_index_d_._plugin_.commands.md#getcommands)
* [registerCommand](_index_d_._plugin_.commands.md#registercommand)
* [registerTextEditorCommand](_index_d_._plugin_.commands.md#registertexteditorcommand)

## Functions

### executeCommand

▸ **executeCommand**\<T>(`command`: string, ...`rest`: any[]): [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

*Defined in [index.d.ts:7182](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7182)*

Executes the command denoted by the given command identifier.

* *Note 1:* When executing an editor command not all types are allowed to
be passed as arguments. Allowed are the primitive types `string`, `boolean`,
`number`, `undefined`, and `null`, as well as [`Position`](#Position), [`Range`](#Range), [`Uri`](#Uri) and [`Location`](#Location).
* *Note 2:* There are no restrictions when executing commands that have been contributed
by extensions.

#### Type parameters:

Name |
------ |
`T` |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`command` | string | Identifier of the command to execute. |
`...rest` | any[] | Parameters passed to the command function. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<T \| undefined>

A thenable that resolves to the returned value of the given command. `undefined` when
the command handler function doesn't return anything.

___

### getCommands

▸ **getCommands**(`filterInternal?`: boolean): [Thenable](../interfaces/_index_d_.thenable.md)\<string[]>

*Defined in [index.d.ts:7191](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7191)*

Retrieve the list of all available commands. Commands starting with an underscore are
treated as internal commands.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`filterInternal?` | boolean | Set `true` to not see internal commands (starting with an underscore) |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<string[]>

Thenable that resolves to a list of command ids.

___

### registerCommand

▸ **registerCommand**(`command`: string, `callback`: (...args: any[]) => any, `thisArg?`: any): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:7150](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7150)*

Registers a command that can be invoked via a keyboard shortcut,
a menu item, an action, or directly.

Registering a command with an existing command identifier twice
will cause an error.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`command` | string | A unique identifier for the command. |
`callback` | (...args: any[]) => any | A command handler function. |
`thisArg?` | any | The `this` context used when invoking the handler function. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

Disposable which unregisters this command on disposal.

___

### registerTextEditorCommand

▸ **registerTextEditorCommand**(`command`: string, `callback`: (textEditor: [TextEditor](../interfaces/_index_d_._plugin_.texteditor.md), edit: [TextEditorEdit](../interfaces/_index_d_._plugin_.texteditoredit.md), ...args: any[]) => void, `thisArg?`: any): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:7166](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L7166)*

Registers a text editor command that can be invoked via a keyboard shortcut,
a menu item, an action, or directly.

Text editor commands are different from ordinary [commands](#commands.registerCommand) as
they only execute when there is an active editor when the command is called. Also, the
command handler of an editor command has access to the active editor and to an
[edit](#TextEditorEdit)-builder.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`command` | string | A unique identifier for the command. |
`callback` | (textEditor: [TextEditor](../interfaces/_index_d_._plugin_.texteditor.md), edit: [TextEditorEdit](../interfaces/_index_d_._plugin_.texteditoredit.md), ...args: any[]) => void | A command handler function with access to an [editor](#TextEditor) and an [edit](#TextEditorEdit). |
`thisArg?` | any | The `this` context used when invoking the handler function. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

Disposable which unregisters this command on disposal.
