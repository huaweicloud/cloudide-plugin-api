**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CodeActionContext

# Interface: CodeActionContext

Contains additional diagnostic information about the context in which
a [code action](#CodeActionProvider.provideCodeActions) is run.

## Hierarchy

* **CodeActionContext**

## Index

### Properties

* [diagnostics](_index_d_._plugin_.codeactioncontext.md#diagnostics)
* [only](_index_d_._plugin_.codeactioncontext.md#only)

## Properties

### diagnostics

• `Readonly` **diagnostics**: ReadonlyArray\<[Diagnostic](../classes/_index_d_._plugin_.diagnostic.md)>

*Defined in [index.d.ts:2114](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2114)*

An array of diagnostics.

___

### only

• `Optional` `Readonly` **only**: [CodeActionKind](../classes/_index_d_._plugin_.codeactionkind.md)

*Defined in [index.d.ts:2121](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2121)*

Requested kind of actions to return.

Actions not of this kind are filtered out before being shown by the [lightbulb](https://code.visualstudio.com/docs/editor/editingevolved#_code-action).
