**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CodeActionKind

# Class: CodeActionKind

Kind of a code action.

Kinds are a hierarchical list of identifiers separated by `.`, e.g. `"refactor.extract.function"`.

Code action kinds are used by VS Code for UI elements such as the refactoring context menu. Users
can also trigger code actions with a specific kind with the `editor.action.codeAction` command.

## Hierarchy

* **CodeActionKind**

## Index

### Constructors

* [constructor](_index_d_._plugin_.codeactionkind.md#constructor)

### Properties

* [value](_index_d_._plugin_.codeactionkind.md#value)
* [Empty](_index_d_._plugin_.codeactionkind.md#empty)
* [QuickFix](_index_d_._plugin_.codeactionkind.md#quickfix)
* [Refactor](_index_d_._plugin_.codeactionkind.md#refactor)
* [RefactorExtract](_index_d_._plugin_.codeactionkind.md#refactorextract)
* [RefactorInline](_index_d_._plugin_.codeactionkind.md#refactorinline)
* [RefactorRewrite](_index_d_._plugin_.codeactionkind.md#refactorrewrite)
* [Source](_index_d_._plugin_.codeactionkind.md#source)
* [SourceFixAll](_index_d_._plugin_.codeactionkind.md#sourcefixall)
* [SourceOrganizeImports](_index_d_._plugin_.codeactionkind.md#sourceorganizeimports)

### Methods

* [append](_index_d_._plugin_.codeactionkind.md#append)
* [contains](_index_d_._plugin_.codeactionkind.md#contains)
* [intersects](_index_d_._plugin_.codeactionkind.md#intersects)

## Constructors

### constructor

\+ `Private`**new CodeActionKind**(`value`: string): [CodeActionKind](_index_d_._plugin_.codeactionkind.md)

*Defined in [index.d.ts:2241](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2241)*

#### Parameters:

Name | Type |
------ | ------ |
`value` | string |

**Returns:** [CodeActionKind](_index_d_._plugin_.codeactionkind.md)

## Properties

### value

• `Readonly` **value**: string

*Defined in [index.d.ts:2248](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2248)*

String value of the kind, e.g. `"refactor.extract.function"`.

___

### Empty

▪ `Static` `Readonly` **Empty**: [CodeActionKind](_index_d_._plugin_.codeactionkind.md)

*Defined in [index.d.ts:2166](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2166)*

Empty kind.

___

### QuickFix

▪ `Static` `Readonly` **QuickFix**: [CodeActionKind](_index_d_._plugin_.codeactionkind.md)

*Defined in [index.d.ts:2173](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2173)*

Base kind for quickfix actions: `quickfix`.

Quick fix actions address a problem in the code and are shown in the normal code action context menu.

___

### Refactor

▪ `Static` `Readonly` **Refactor**: [CodeActionKind](_index_d_._plugin_.codeactionkind.md)

*Defined in [index.d.ts:2180](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2180)*

Base kind for refactoring actions: `refactor`

Refactoring actions are shown in the refactoring context menu.

___

### RefactorExtract

▪ `Static` `Readonly` **RefactorExtract**: [CodeActionKind](_index_d_._plugin_.codeactionkind.md)

*Defined in [index.d.ts:2193](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2193)*

Base kind for refactoring extraction actions: `refactor.extract`

Example extract actions:

- Extract method
- Extract function
- Extract variable
- Extract interface from class
- ...

___

### RefactorInline

▪ `Static` `Readonly` **RefactorInline**: [CodeActionKind](_index_d_._plugin_.codeactionkind.md)

*Defined in [index.d.ts:2205](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2205)*

Base kind for refactoring inline actions: `refactor.inline`

Example inline actions:

- Inline function
- Inline variable
- Inline constant
- ...

___

### RefactorRewrite

▪ `Static` `Readonly` **RefactorRewrite**: [CodeActionKind](_index_d_._plugin_.codeactionkind.md)

*Defined in [index.d.ts:2219](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2219)*

Base kind for refactoring rewrite actions: `refactor.rewrite`

Example rewrite actions:

- Convert JavaScript function to class
- Add or remove parameter
- Encapsulate field
- Make method static
- Move method to base class
- ...

___

### Source

▪ `Static` `Readonly` **Source**: [CodeActionKind](_index_d_._plugin_.codeactionkind.md)

*Defined in [index.d.ts:2228](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2228)*

Base kind for source actions: `source`

Source code actions apply to the entire file. They must be explicitly requested and will not show in the
normal [lightbulb](https://code.visualstudio.com/docs/editor/editingevolved#_code-action) menu. Source actions
can be run on save using `editor.codeActionsOnSave` and are also shown in the `source` context menu.

___

### SourceFixAll

▪ `Static` `Readonly` **SourceFixAll**: [CodeActionKind](_index_d_._plugin_.codeactionkind.md)

*Defined in [index.d.ts:2241](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2241)*

Base kind for auto-fix source actions: `source.fixAll`.

Fix all actions automatically fix errors that have a clear fix that do not require user input.
They should not suppress errors or perform unsafe fixes such as generating new types or classes.

___

### SourceOrganizeImports

▪ `Static` `Readonly` **SourceOrganizeImports**: [CodeActionKind](_index_d_._plugin_.codeactionkind.md)

*Defined in [index.d.ts:2233](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2233)*

Base kind for an organize imports source action: `source.organizeImports`.

## Methods

### append

▸ **append**(`parts`: string): [CodeActionKind](_index_d_._plugin_.codeactionkind.md)

*Defined in [index.d.ts:2255](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2255)*

Create a new kind by appending a more specific selector to the current kind.

Does not modify the current kind.

#### Parameters:

Name | Type |
------ | ------ |
`parts` | string |

**Returns:** [CodeActionKind](_index_d_._plugin_.codeactionkind.md)

___

### contains

▸ **contains**(`other`: [CodeActionKind](_index_d_._plugin_.codeactionkind.md)): boolean

*Defined in [index.d.ts:2275](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2275)*

Checks if `other` is a sub-kind of this `CodeActionKind`.

The kind `"refactor.extract"` for example contains `"refactor.extract"` and ``"refactor.extract.function"`,
but not `"unicorn.refactor.extract"`, or `"refactor.extractAll"` or `refactor`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`other` | [CodeActionKind](_index_d_._plugin_.codeactionkind.md) | Kind to check.  |

**Returns:** boolean

___

### intersects

▸ **intersects**(`other`: [CodeActionKind](_index_d_._plugin_.codeactionkind.md)): boolean

*Defined in [index.d.ts:2265](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L2265)*

Checks if this code action kind intersects `other`.

The kind `"refactor.extract"` for example intersects `refactor`, `"refactor.extract"` and ``"refactor.extract.function"`,
but not `"unicorn.refactor.extract"`, or `"refactor.extractAll"`.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`other` | [CodeActionKind](_index_d_._plugin_.codeactionkind.md) | Kind to check.  |

**Returns:** boolean
