[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CodeAction

# Class: CodeAction

["@codearts/plugin"](../modules/_codearts_plugin_.md).CodeAction

A code action represents a change that can be performed in code, e.g. to fix a problem or
to refactor code.

A CodeAction must set either [`edit`](codearts_plugin_.CodeAction.md#edit) and/or a [`command`](codearts_plugin_.CodeAction.md#command). If both are supplied, the `edit` is applied first, then the command is executed.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.CodeAction.md#constructor)

### Properties

- [command](codearts_plugin_.CodeAction.md#command)
- [diagnostics](codearts_plugin_.CodeAction.md#diagnostics)
- [disabled](codearts_plugin_.CodeAction.md#disabled)
- [edit](codearts_plugin_.CodeAction.md#edit)
- [isPreferred](codearts_plugin_.CodeAction.md#ispreferred)
- [kind](codearts_plugin_.CodeAction.md#kind)
- [title](codearts_plugin_.CodeAction.md#title)

## Constructors

### constructor

• **new CodeAction**(`title`, `kind?`)

Creates a new code action.

A code action must have at least a [title](codearts_plugin_.CodeAction.md#title) and [edits](codearts_plugin_.CodeAction.md#edit)
and/or a [command](codearts_plugin_.CodeAction.md#command).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `title` | `string` | The title of the code action. |
| `kind?` | [`CodeActionKind`](codearts_plugin_.CodeActionKind.md) | The kind of the code action. |

#### Defined in

[index.d.ts:2477](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L2477)

## Properties

### command

• `Optional` **command**: [`Command`](../interfaces/codearts_plugin_.Command.md)

A [Command](../interfaces/codearts_plugin_.Command.md) this code action executes.

If this command throws an exception, the editor displays the exception message to users in the editor at the
current cursor position.

#### Defined in

[index.d.ts:2428](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L2428)

___

### diagnostics

• `Optional` **diagnostics**: [`Diagnostic`](codearts_plugin_.Diagnostic.md)[]

[Diagnostics](codearts_plugin_.Diagnostic.md) that this code action resolves.

#### Defined in

[index.d.ts:2420](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L2420)

___

### disabled

• `Optional` **disabled**: `Object`

Marks that the code action cannot currently be applied.

- Disabled code actions are not shown in automatic [lightbulb](https://code.visualstudio.com/docs/editor/editingevolved#_code-action)
code action menu.

- Disabled actions are shown as faded out in the code action menu when the user request a more specific type
of code action, such as refactorings.

- If the user has a [keybinding](https://code.visualstudio.com/docs/editor/refactoring#_keybindings-for-code-actions)
that auto applies a code action and only a disabled code actions are returned, the editor will show the user an
error message with `reason` in the editor.

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `reason` | `string` | Human readable description of why the code action is currently disabled.  This is displayed in the code actions UI. |

#### Defined in

[index.d.ts:2459](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L2459)

___

### edit

• `Optional` **edit**: [`WorkspaceEdit`](codearts_plugin_.WorkspaceEdit.md)

A [workspace edit](codearts_plugin_.WorkspaceEdit.md) this code action performs.

#### Defined in

[index.d.ts:2415](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L2415)

___

### isPreferred

• `Optional` **isPreferred**: `boolean`

Marks this as a preferred action. Preferred actions are used by the `auto fix` command and can be targeted
by keybindings.

A quick fix should be marked preferred if it properly addresses the underlying error.
A refactoring should be marked preferred if it is the most reasonable choice of actions to take.

#### Defined in

[index.d.ts:2444](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L2444)

___

### kind

• `Optional` **kind**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

[Kind](codearts_plugin_.CodeActionKind.md) of the code action.

Used to filter code actions.

#### Defined in

[index.d.ts:2435](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L2435)

___

### title

• **title**: `string`

A short, human-readable, title for this code action.

#### Defined in

[index.d.ts:2410](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L2410)
