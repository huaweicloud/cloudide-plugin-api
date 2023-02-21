[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CodeActionKind

# Class: CodeActionKind

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CodeActionKind

Kind of a code action.

Kinds are a hierarchical list of identifiers separated by `.`, e.g. `"refactor.extract.function"`.

Code action kinds are used by VS Code for UI elements such as the refactoring context menu. Users
can also trigger code actions with a specific kind with the `editor.action.codeAction` command.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.CodeActionKind.md#constructor)

### Properties

- [value](cloudide_plugin_.CodeActionKind.md#value)
- [Empty](cloudide_plugin_.CodeActionKind.md#empty)
- [QuickFix](cloudide_plugin_.CodeActionKind.md#quickfix)
- [Refactor](cloudide_plugin_.CodeActionKind.md#refactor)
- [RefactorExtract](cloudide_plugin_.CodeActionKind.md#refactorextract)
- [RefactorInline](cloudide_plugin_.CodeActionKind.md#refactorinline)
- [RefactorRewrite](cloudide_plugin_.CodeActionKind.md#refactorrewrite)
- [Source](cloudide_plugin_.CodeActionKind.md#source)
- [SourceOrganizeImports](cloudide_plugin_.CodeActionKind.md#sourceorganizeimports)

### Methods

- [append](cloudide_plugin_.CodeActionKind.md#append)
- [contains](cloudide_plugin_.CodeActionKind.md#contains)
- [intersects](cloudide_plugin_.CodeActionKind.md#intersects)

## Constructors

### constructor

• `Private` **new CodeActionKind**(`value`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Defined in

[index.d.ts:8157](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8157)

## Properties

### value

• `Optional` `Readonly` **value**: `string`

String value of the kind, e.g. `"refactor.extract.function"`.

#### Defined in

[index.d.ts:8162](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8162)

___

### Empty

▪ `Static` `Readonly` **Empty**: [`CodeActionKind`](cloudide_plugin_.CodeActionKind.md)

Empty kind.

#### Defined in

[index.d.ts:8089](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8089)

___

### QuickFix

▪ `Static` `Readonly` **QuickFix**: [`CodeActionKind`](cloudide_plugin_.CodeActionKind.md)

Base kind for quickfix actions: `quickfix`.

Quick fix actions address a problem in the code and are shown in the normal code action context menu.

#### Defined in

[index.d.ts:8096](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8096)

___

### Refactor

▪ `Static` `Readonly` **Refactor**: [`CodeActionKind`](cloudide_plugin_.CodeActionKind.md)

Base kind for refactoring actions: `refactor`

Refactoring actions are shown in the refactoring context menu.

#### Defined in

[index.d.ts:8103](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8103)

___

### RefactorExtract

▪ `Static` `Readonly` **RefactorExtract**: [`CodeActionKind`](cloudide_plugin_.CodeActionKind.md)

Base kind for refactoring extraction actions: `refactor.extract`

Example extract actions:

- Extract method
- Extract function
- Extract variable
- Extract interface from class
- ...

#### Defined in

[index.d.ts:8116](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8116)

___

### RefactorInline

▪ `Static` `Readonly` **RefactorInline**: [`CodeActionKind`](cloudide_plugin_.CodeActionKind.md)

Base kind for refactoring inline actions: `refactor.inline`

Example inline actions:

- Inline function
- Inline variable
- Inline constant
- ...

#### Defined in

[index.d.ts:8128](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8128)

___

### RefactorRewrite

▪ `Static` `Readonly` **RefactorRewrite**: [`CodeActionKind`](cloudide_plugin_.CodeActionKind.md)

Base kind for refactoring rewrite actions: `refactor.rewrite`

Example rewrite actions:

- Convert JavaScript function to class
- Add or remove parameter
- Encapsulate field
- Make method static
- Move method to base class
- ...

#### Defined in

[index.d.ts:8142](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8142)

___

### Source

▪ `Static` `Readonly` **Source**: [`CodeActionKind`](cloudide_plugin_.CodeActionKind.md)

Base kind for source actions: `source`

Source code actions apply to the entire file and can be run on save
using `editor.codeActionsOnSave`. They also are shown in `source` context menu.

#### Defined in

[index.d.ts:8150](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8150)

___

### SourceOrganizeImports

▪ `Static` `Readonly` **SourceOrganizeImports**: [`CodeActionKind`](cloudide_plugin_.CodeActionKind.md)

Base kind for an organize imports source action: `source.organizeImports`.

#### Defined in

[index.d.ts:8155](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8155)

## Methods

### append

▸ **append**(`parts`): [`CodeActionKind`](cloudide_plugin_.CodeActionKind.md)

Create a new kind by appending a more specific selector to the current kind.

Does not modify the current kind.

#### Parameters

| Name | Type |
| :------ | :------ |
| `parts` | `string` |

#### Returns

[`CodeActionKind`](cloudide_plugin_.CodeActionKind.md)

#### Defined in

[index.d.ts:8169](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8169)

___

### contains

▸ **contains**(`other`): `boolean`

Does this kind contain `other`?

The kind `"refactor"` for example contains `"refactor.extract"` and ``"refactor.extract.function"`, but not `"unicorn.refactor.extract"` or `"refactory.extract"`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`CodeActionKind`](cloudide_plugin_.CodeActionKind.md) | Kind to check. |

#### Returns

`boolean`

#### Defined in

[index.d.ts:8178](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8178)

___

### intersects

▸ **intersects**(`other`): `boolean`

Check if this code action kind intersects `other`.
The kind "refactor.extract" for example intersects refactor, "refactor.extract" and
`"refactor.extract.function", but not "unicorn.refactor.extract", or "refactor.extractAll".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`CodeActionKind`](cloudide_plugin_.CodeActionKind.md) | Kind to check. |

#### Returns

`boolean`

#### Defined in

[index.d.ts:8187](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8187)
