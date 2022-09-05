[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / commands

# Namespace: commands

["@codearts/plugin"](_codearts_plugin_.md).commands

Namespace for dealing with commands. In short, a command is a function with a
unique identifier. The function is sometimes also called _command handler_.

Commands can be added to the editor using the [registerCommand](codearts_plugin_.commands.md#registercommand)
and [registerTextEditorCommand](codearts_plugin_.commands.md#registertexteditorcommand) functions. Commands
can be executed [manually](codearts_plugin_.commands.md#executecommand) or from a UI gesture. Those are:

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

## Table of contents

### Functions

- [executeCommand](codearts_plugin_.commands.md#executecommand)
- [getCommands](codearts_plugin_.commands.md#getcommands)
- [registerCommand](codearts_plugin_.commands.md#registercommand)
- [registerTextEditorCommand](codearts_plugin_.commands.md#registertexteditorcommand)

## Functions

### executeCommand

▸ **executeCommand**<`T`\>(`command`, ...`rest`): [`Thenable`](../interfaces/Thenable.md)<`T`\>

Executes the command denoted by the given command identifier.

* *Note 1:* When executing an editor command not all types are allowed to
be passed as arguments. Allowed are the primitive types `string`, `boolean`,
`number`, `undefined`, and `null`, as well as [`Position`](../classes/codearts_plugin_.Position.md), [`Range`](../classes/codearts_plugin_.Range.md), [`Uri`](../classes/codearts_plugin_.Uri.md) and [`Location`](../classes/codearts_plugin_.Location.md).
* *Note 2:* There are no restrictions when executing commands that have been contributed
by extensions.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `unknown` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `command` | `string` | Identifier of the command to execute. |
| `...rest` | `any`[] | Parameters passed to the command function. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T`\>

A thenable that resolves to the returned value of the given command. Returns `undefined` when
the command handler function doesn't return anything.

#### Defined in

[index.d.ts:9255](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9255)

___

### getCommands

▸ **getCommands**(`filterInternal?`): [`Thenable`](../interfaces/Thenable.md)<`string`[]\>

Retrieve the list of all available commands. Commands starting with an underscore are
treated as internal commands.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `filterInternal?` | `boolean` | Set `true` to not see internal commands (starting with an underscore) |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`string`[]\>

Thenable that resolves to a list of command ids.

#### Defined in

[index.d.ts:9264](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9264)

___

### registerCommand

▸ **registerCommand**(`command`, `callback`, `thisArg?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Registers a command that can be invoked via a keyboard shortcut,
a menu item, an action, or directly.

Registering a command with an existing command identifier twice
will cause an error.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `command` | `string` | A unique identifier for the command. |
| `callback` | (...`args`: `any`[]) => `any` | A command handler function. |
| `thisArg?` | `any` | The `this` context used when invoking the handler function. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

Disposable which unregisters this command on disposal.

#### Defined in

[index.d.ts:9222](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9222)

___

### registerTextEditorCommand

▸ **registerTextEditorCommand**(`command`, `callback`, `thisArg?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Registers a text editor command that can be invoked via a keyboard shortcut,
a menu item, an action, or directly.

Text editor commands are different from ordinary [commands](codearts_plugin_.commands.md#registercommand) as
they only execute when there is an active editor when the command is called. Also, the
command handler of an editor command has access to the active editor and to an
[edit](../interfaces/codearts_plugin_.TextEditorEdit.md)-builder. Note that the edit-builder is only valid while the
callback executes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `command` | `string` | A unique identifier for the command. |
| `callback` | (`textEditor`: [`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md), `edit`: [`TextEditorEdit`](../interfaces/codearts_plugin_.TextEditorEdit.md), ...`args`: `any`[]) => `void` | A command handler function with access to an [editor](../interfaces/codearts_plugin_.TextEditor.md) and an [edit](../interfaces/codearts_plugin_.TextEditorEdit.md). |
| `thisArg?` | `any` | The `this` context used when invoking the handler function. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

Disposable which unregisters this command on disposal.

#### Defined in

[index.d.ts:9239](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L9239)
