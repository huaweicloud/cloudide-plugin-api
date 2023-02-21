[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CodeActionContext

# Interface: CodeActionContext

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CodeActionContext

Contains additional diagnostic information about the context in which
a [code action](#CodeActionProvider.provideCodeActions) is run.

## Table of contents

### Properties

- [diagnostics](cloudide_plugin_.CodeActionContext.md#diagnostics)
- [only](cloudide_plugin_.CodeActionContext.md#only)

## Properties

### diagnostics

• `Readonly` **diagnostics**: [`Diagnostic`](../classes/cloudide_plugin_.Diagnostic.md)[]

An array of diagnostics.

#### Defined in

[index.d.ts:8198](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8198)

___

### only

• `Optional` `Readonly` **only**: [`CodeActionKind`](../classes/cloudide_plugin_.CodeActionKind.md)

Requested kind of actions to return.

Actions not of this kind are filtered out before being shown by the lightbulb.

#### Defined in

[index.d.ts:8205](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8205)
