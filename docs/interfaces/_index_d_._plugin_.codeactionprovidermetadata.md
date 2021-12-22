**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CodeActionProviderMetadata

# Interface: CodeActionProviderMetadata

Metadata about the type of code actions that a [CodeActionProvider](#CodeActionProvider) provides.

## Hierarchy

* **CodeActionProviderMetadata**

## Index

### Properties

* [documentation](_index_d_._plugin_.codeactionprovidermetadata.md#documentation)
* [providedCodeActionKinds](_index_d_._plugin_.codeactionprovidermetadata.md#providedcodeactionkinds)

## Properties

### documentation

• `Optional` `Readonly` **documentation**: ReadonlyArray\<{ command: [Command](_index_d_._plugin_.command.md) ; kind: [CodeActionKind](../classes/_index_d_._plugin_.codeactionkind.md)  }>

*Defined in [index.d.ts:2445](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2445)*

Static documentation for a class of code actions.

Documentation from the provider is shown in the code actions menu if either:

- Code actions of `kind` are requested by VS Code. In this case, VS Code will show the documentation that
  most closely matches the requested code action kind. For example, if a provider has documentation for
  both `Refactor` and `RefactorExtract`, when the user requests code actions for `RefactorExtract`,
  VS Code will use the documentation for `RefactorExtract` instead of the documentation for `Refactor`.

- Any code actions of `kind` are returned by the provider.

At most one documentation entry will be shown per provider.

___

### providedCodeActionKinds

• `Optional` `Readonly` **providedCodeActionKinds**: ReadonlyArray\<[CodeActionKind](../classes/_index_d_._plugin_.codeactionkind.md)>

*Defined in [index.d.ts:2429](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L2429)*

List of [CodeActionKinds](#CodeActionKind) that a [CodeActionProvider](#CodeActionProvider) may return.

This list is used to determine if a given `CodeActionProvider` should be invoked or not.
To avoid unnecessary computation, every `CodeActionProvider` should list use `providedCodeActionKinds`. The
list of kinds may either be generic, such as `[CodeActionKind.Refactor]`, or list out every kind provided,
such as `[CodeActionKind.Refactor.Extract.append('function'), CodeActionKind.Refactor.Extract.append('constant'), ...]`.
