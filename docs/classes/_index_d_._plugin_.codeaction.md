**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CodeAction

# Class: CodeAction

A code action represents a change that can be performed in code, e.g. to fix a problem or
to refactor code.

A CodeAction must set either [`edit`](#CodeAction.edit) and/or a [`command`](#CodeAction.command). If both are supplied, the `edit` is applied first, then the command is executed.

## Hierarchy

* **CodeAction**

## Index

### Constructors

* [constructor](_index_d_._plugin_.codeaction.md#constructor)

### Properties

* [command](_index_d_._plugin_.codeaction.md#command)
* [diagnostics](_index_d_._plugin_.codeaction.md#diagnostics)
* [disabled](_index_d_._plugin_.codeaction.md#disabled)
* [edit](_index_d_._plugin_.codeaction.md#edit)
* [isPreferred](_index_d_._plugin_.codeaction.md#ispreferred)
* [kind](_index_d_._plugin_.codeaction.md#kind)
* [title](_index_d_._plugin_.codeaction.md#title)

## Constructors

### constructor

\+ **new CodeAction**(`title`: string, `kind?`: [CodeActionKind](_index_d_._plugin_.codeactionkind.md)): [CodeAction](_index_d_._plugin_.codeaction.md)

*Defined in [index.d.ts:2366](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2366)*

Creates a new code action.

A code action must have at least a [title](#CodeAction.title) and [edits](#CodeAction.edit)
and/or a [command](#CodeAction.command).

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`title` | string | The title of the code action. |
`kind?` | [CodeActionKind](_index_d_._plugin_.codeactionkind.md) | The kind of the code action.  |

**Returns:** [CodeAction](_index_d_._plugin_.codeaction.md)

## Properties

### command

• `Optional` **command**: [Command](../interfaces/_index_d_._plugin_.command.md)

*Defined in [index.d.ts:2328](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2328)*

A [command](#Command) this code action executes.

If this command throws an exception, VS Code displays the exception message to users in the editor at the
current cursor position.

___

### diagnostics

• `Optional` **diagnostics**: [Diagnostic](_index_d_._plugin_.diagnostic.md)[]

*Defined in [index.d.ts:2320](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2320)*

[Diagnostics](#Diagnostic) that this code action resolves.

___

### disabled

• `Optional` **disabled**: { reason: string  }

*Defined in [index.d.ts:2359](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2359)*

Marks that the code action cannot currently be applied.

- Disabled code actions are not shown in automatic [lightbulb](https://code.visualstudio.com/docs/editor/editingevolved#_code-action)
code action menu.

- Disabled actions are shown as faded out in the code action menu when the user request a more specific type
of code action, such as refactorings.

- If the user has a [keybinding](https://code.visualstudio.com/docs/editor/refactoring#_keybindings-for-code-actions)
that auto applies a code action and only a disabled code actions are returned, VS Code will show the user an
error message with `reason` in the editor.

#### Type declaration:

Name | Type | Description |
------ | ------ | ------ |
`reason` | string | Human readable description of why the code action is currently disabled.  This is displayed in the code actions UI.  |

___

### edit

• `Optional` **edit**: [WorkspaceEdit](_index_d_._plugin_.workspaceedit.md)

*Defined in [index.d.ts:2315](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2315)*

A [workspace edit](#WorkspaceEdit) this code action performs.

___

### isPreferred

• `Optional` **isPreferred**: boolean

*Defined in [index.d.ts:2344](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2344)*

Marks this as a preferred action. Preferred actions are used by the `auto fix` command and can be targeted
by keybindings.

A quick fix should be marked preferred if it properly addresses the underlying error.
A refactoring should be marked preferred if it is the most reasonable choice of actions to take.

___

### kind

• `Optional` **kind**: [CodeActionKind](_index_d_._plugin_.codeactionkind.md)

*Defined in [index.d.ts:2335](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2335)*

[Kind](#CodeActionKind) of the code action.

Used to filter code actions.

___

### title

•  **title**: string

*Defined in [index.d.ts:2310](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2310)*

A short, human-readable, title for this code action.
