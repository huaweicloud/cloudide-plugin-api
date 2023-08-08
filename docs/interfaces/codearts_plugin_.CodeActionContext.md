[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CodeActionContext

# Interface: CodeActionContext

["@codearts/plugin"](../modules/_codearts_plugin_.md).CodeActionContext

Contains additional diagnostic information about the context in which
a [code action](codearts_plugin_.CodeActionProvider.md#providecodeactions) is run.

## Table of contents

### Properties

- [diagnostics](codearts_plugin_.CodeActionContext.md#diagnostics)
- [only](codearts_plugin_.CodeActionContext.md#only)
- [triggerKind](codearts_plugin_.CodeActionContext.md#triggerkind)

## Properties

### diagnostics

• `Readonly` **diagnostics**: readonly [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]

An array of diagnostics.

#### Defined in

[index.d.ts:2389](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2389)

___

### only

• `Readonly` **only**: `undefined` \| [`CodeActionKind`](../classes/codearts_plugin_.CodeActionKind.md)

Requested kind of actions to return.

Actions not of this kind are filtered out before being shown by the [lightbulb](https://code.visualstudio.com/docs/editor/editingevolved#_code-action).

#### Defined in

[index.d.ts:2396](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2396)

___

### triggerKind

• `Readonly` **triggerKind**: [`CodeActionTriggerKind`](../enums/codearts_plugin_.CodeActionTriggerKind.md)

The reason why code actions were requested.

#### Defined in

[index.d.ts:2384](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2384)
