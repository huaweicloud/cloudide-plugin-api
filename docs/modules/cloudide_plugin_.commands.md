[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](_cloudide_plugin_.md) / commands

# Namespace: commands

["@cloudide/plugin"](_cloudide_plugin_.md).commands

Namespace for dealing with commands. In short, a command is a function with a
unique identifier. The function is sometimes also called _command handler_.

Commands can be added using the [registerCommand](#commands.registerCommand) and
[registerTextEditorCommand](#commands.registerTextEditorCommand) functions.
Registration can be split in two step: first register command without handler,
second register handler by command id.

Any contributed command are available to any plugin, command can be invoked
by [executeCommand](#commands.executeCommand) function.

Simple example that register command:
```javascript
theia.commands.registerCommand({id:'say.hello.command'}, ()=>{
    console.log("Hello World!");
});
```

Simple example that invoke command:

```javascript
theia.commands.executeCommand('core.about');
```

## Table of contents

### Functions

- [executeCommand](cloudide_plugin_.commands.md#executecommand)
- [getCommands](cloudide_plugin_.commands.md#getcommands)
- [registerCommand](cloudide_plugin_.commands.md#registercommand)
- [registerHandler](cloudide_plugin_.commands.md#registerhandler)
- [registerTextEditorCommand](cloudide_plugin_.commands.md#registertexteditorcommand)

## Functions

### executeCommand

▸ **executeCommand**<`T`\>(`commandId`, `...args`): `PromiseLike`<`T` \| `undefined`\>

Execute the active handler for the given command and arguments.

Reject if a command cannot be executed.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `commandId` | `string` |
| `...args` | `any`[] |

#### Returns

`PromiseLike`<`T` \| `undefined`\>

#### Defined in

[index.d.ts:2434](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2434)

___

### getCommands

▸ **getCommands**(`filterInternal?`): `PromiseLike`<`string`[]\>

Retrieve the list of all available commands. Commands starting an underscore are
treated as internal commands.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `filterInternal?` | `boolean` | Set `true` to not see internal commands (starting with an underscore) |

#### Returns

`PromiseLike`<`string`[]\>

Thenable that resolves to a list of command ids.

#### Defined in

[index.d.ts:2443](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2443)

___

### registerCommand

▸ **registerCommand**(`command`, `handler?`, `thisArg?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register the given command and handler if present.

Throw if a command is already registered for the given command identifier.

#### Parameters

| Name | Type |
| :------ | :------ |
| `command` | `string` \| [`CommandDescription`](../interfaces/cloudide_plugin_.CommandDescription.md) |
| `handler?` | (...`args`: `any`[]) => `any` |
| `thisArg?` | `any` |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Defined in

[index.d.ts:2401](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2401)

___

### registerHandler

▸ **registerHandler**(`commandId`, `handler`, `thisArg?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register the given handler for the given command identifier.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `commandId` | `string` | a given command id |
| `handler` | (...`args`: `any`[]) => `any` | a command handler Throw if a handler for the given command identifier is already registered. |
| `thisArg?` | `any` | - |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Defined in

[index.d.ts:2411](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2411)

___

### registerTextEditorCommand

▸ **registerTextEditorCommand**(`command`, `callback`, `thisArg?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Registers a text editor command that can be invoked via a keyboard shortcut,
a menu item, an action, or directly.

Text editor commands are different from ordinary [commands](#commands.registerCommand) as
they only execute when there is an active editor when the command is called. Also, the
command handler of an editor command has access to the active editor and to an
[edit](#TextEditorEdit)-builder.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `command` | `string` | A unique identifier for the command. |
| `callback` | (`textEditor`: [`TextEditor`](../interfaces/cloudide_plugin_.TextEditor.md), `edit`: [`TextEditorEdit`](../interfaces/cloudide_plugin_.TextEditorEdit.md), ...`args`: `any`[]) => `void` | A command handler function with access to an [editor](#TextEditor) and an [edit](#TextEditorEdit). |
| `thisArg?` | `any` | The `this` context used when invoking the handler function. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Disposable which unregisters this command on disposal.

#### Defined in

[index.d.ts:2427](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2427)
