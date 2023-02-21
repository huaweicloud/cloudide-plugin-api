[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CodeAction

# Class: CodeAction

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CodeAction

A code action represents a change that can be performed in code, e.g. to fix a problem or
to refactor code.

A CodeAction must set either [`edit`](#edit) and/or a [`command`](#command).
If both are supplied, the `edit` is applied first, then the command is executed.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.CodeAction.md#constructor)

### Properties

- [command](cloudide_plugin_.CodeAction.md#command)
- [diagnostics](cloudide_plugin_.CodeAction.md#diagnostics)
- [edit](cloudide_plugin_.CodeAction.md#edit)
- [kind](cloudide_plugin_.CodeAction.md#kind)
- [title](cloudide_plugin_.CodeAction.md#title)

## Constructors

### constructor

• **new CodeAction**(`title`, `kind?`)

Creates a new code action.

A code action must have at least a [title](#CodeAction.title) and [edits](#CodeAction.edit)
and/or a [command](#CodeAction.command).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `title` | `string` | The title of the code action. |
| `kind?` | [`CodeActionKind`](cloudide_plugin_.CodeActionKind.md) | The kind of the code action. |

#### Defined in

[index.d.ts:7968](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7968)

## Properties

### command

• `Optional` **command**: [`Command`](../interfaces/cloudide_plugin_.Command.md)

A [command](#Command) this code action executes.

#### Defined in

[index.d.ts:7950](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7950)

___

### diagnostics

• `Optional` **diagnostics**: [`Diagnostic`](cloudide_plugin_.Diagnostic.md)[]

[Diagnostics](#Diagnostic) that this code action resolves.

#### Defined in

[index.d.ts:7940](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7940)

___

### edit

• `Optional` **edit**: [`WorkspaceEdit`](cloudide_plugin_.WorkspaceEdit.md)

A [workspace edit](#WorkspaceEdit) this code action performs.

#### Defined in

[index.d.ts:7945](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7945)

___

### kind

• `Optional` **kind**: [`CodeActionKind`](cloudide_plugin_.CodeActionKind.md)

[Kind](#CodeActionKind) of the code action.

Used to filter code actions.

#### Defined in

[index.d.ts:7957](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7957)

___

### title

• **title**: `string`

A short, human-readable, title for this code action.

#### Defined in

[index.d.ts:7935](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7935)
