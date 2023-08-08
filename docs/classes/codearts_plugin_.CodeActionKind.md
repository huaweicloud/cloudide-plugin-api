[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CodeActionKind

# Class: CodeActionKind

["@codearts/plugin"](../modules/_codearts_plugin_.md).CodeActionKind

Kind of a code action.

Kinds are a hierarchical list of identifiers separated by `.`, e.g. `"refactor.extract.function"`.

Code action kinds are used by the editor for UI elements such as the refactoring context menu. Users
can also trigger code actions with a specific kind with the `editor.action.codeAction` command.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.CodeActionKind.md#constructor)

### Properties

- [value](codearts_plugin_.CodeActionKind.md#value)
- [Empty](codearts_plugin_.CodeActionKind.md#empty)
- [QuickFix](codearts_plugin_.CodeActionKind.md#quickfix)
- [Refactor](codearts_plugin_.CodeActionKind.md#refactor)
- [RefactorExtract](codearts_plugin_.CodeActionKind.md#refactorextract)
- [RefactorInline](codearts_plugin_.CodeActionKind.md#refactorinline)
- [RefactorRewrite](codearts_plugin_.CodeActionKind.md#refactorrewrite)
- [Source](codearts_plugin_.CodeActionKind.md#source)
- [SourceFixAll](codearts_plugin_.CodeActionKind.md#sourcefixall)
- [SourceOrganizeImports](codearts_plugin_.CodeActionKind.md#sourceorganizeimports)

### Methods

- [append](codearts_plugin_.CodeActionKind.md#append)
- [contains](codearts_plugin_.CodeActionKind.md#contains)
- [intersects](codearts_plugin_.CodeActionKind.md#intersects)

## Constructors

### constructor

• `Private` **new CodeActionKind**(`value`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Defined in

[index.d.ts:2323](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2323)

## Properties

### value

• `Readonly` **value**: `string`

String value of the kind, e.g. `"refactor.extract.function"`.

#### Defined in

[index.d.ts:2328](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2328)

___

### Empty

▪ `Static` `Readonly` **Empty**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

Empty kind.

#### Defined in

[index.d.ts:2246](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2246)

___

### QuickFix

▪ `Static` `Readonly` **QuickFix**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

Base kind for quickfix actions: `quickfix`.

Quick fix actions address a problem in the code and are shown in the normal code action context menu.

#### Defined in

[index.d.ts:2253](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2253)

___

### Refactor

▪ `Static` `Readonly` **Refactor**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

Base kind for refactoring actions: `refactor`

Refactoring actions are shown in the refactoring context menu.

#### Defined in

[index.d.ts:2260](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2260)

___

### RefactorExtract

▪ `Static` `Readonly` **RefactorExtract**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

Base kind for refactoring extraction actions: `refactor.extract`

Example extract actions:

- Extract method
- Extract function
- Extract variable
- Extract interface from class
- ...

#### Defined in

[index.d.ts:2273](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2273)

___

### RefactorInline

▪ `Static` `Readonly` **RefactorInline**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

Base kind for refactoring inline actions: `refactor.inline`

Example inline actions:

- Inline function
- Inline variable
- Inline constant
- ...

#### Defined in

[index.d.ts:2285](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2285)

___

### RefactorRewrite

▪ `Static` `Readonly` **RefactorRewrite**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

Base kind for refactoring rewrite actions: `refactor.rewrite`

Example rewrite actions:

- Convert JavaScript function to class
- Add or remove parameter
- Encapsulate field
- Make method static
- Move method to base class
- ...

#### Defined in

[index.d.ts:2299](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2299)

___

### Source

▪ `Static` `Readonly` **Source**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

Base kind for source actions: `source`

Source code actions apply to the entire file. They must be explicitly requested and will not show in the
normal [lightbulb](https://code.visualstudio.com/docs/editor/editingevolved#_code-action) menu. Source actions
can be run on save using `editor.codeActionsOnSave` and are also shown in the `source` context menu.

#### Defined in

[index.d.ts:2308](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2308)

___

### SourceFixAll

▪ `Static` `Readonly` **SourceFixAll**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

Base kind for auto-fix source actions: `source.fixAll`.

Fix all actions automatically fix errors that have a clear fix that do not require user input.
They should not suppress errors or perform unsafe fixes such as generating new types or classes.

#### Defined in

[index.d.ts:2321](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2321)

___

### SourceOrganizeImports

▪ `Static` `Readonly` **SourceOrganizeImports**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

Base kind for an organize imports source action: `source.organizeImports`.

#### Defined in

[index.d.ts:2313](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2313)

## Methods

### append

▸ **append**(`parts`): [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

Create a new kind by appending a more specific selector to the current kind.

Does not modify the current kind.

#### Parameters

| Name | Type |
| :------ | :------ |
| `parts` | `string` |

#### Returns

[`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

#### Defined in

[index.d.ts:2335](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2335)

___

### contains

▸ **contains**(`other`): `boolean`

Checks if `other` is a sub-kind of this `CodeActionKind`.

The kind `"refactor.extract"` for example contains `"refactor.extract"` and ``"refactor.extract.function"`,
but not `"unicorn.refactor.extract"`, or `"refactor.extractAll"` or `refactor`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`CodeActionKind`](codearts_plugin_.CodeActionKind.md) | Kind to check. |

#### Returns

`boolean`

#### Defined in

[index.d.ts:2355](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2355)

___

### intersects

▸ **intersects**(`other`): `boolean`

Checks if this code action kind intersects `other`.

The kind `"refactor.extract"` for example intersects `refactor`, `"refactor.extract"` and ``"refactor.extract.function"`,
but not `"unicorn.refactor.extract"`, or `"refactor.extractAll"`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`CodeActionKind`](codearts_plugin_.CodeActionKind.md) | Kind to check. |

#### Returns

`boolean`

#### Defined in

[index.d.ts:2345](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2345)
