[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CodeActionProviderMetadata

# Interface: CodeActionProviderMetadata

["@codearts/plugin"](../modules/_codearts_plugin_.md).CodeActionProviderMetadata

Metadata about the type of code actions that a [CodeActionProvider](codearts_plugin_.CodeActionProvider.md) provides.

## Table of contents

### Properties

- [documentation](codearts_plugin_.CodeActionProviderMetadata.md#documentation)
- [providedCodeActionKinds](codearts_plugin_.CodeActionProviderMetadata.md#providedcodeactionkinds)

## Properties

### documentation

• `Optional` `Readonly` **documentation**: readonly { `command`: [`Command`](codearts_plugin_.Command.md) ; `kind`: [`CodeActionKind`](../classes/codearts_plugin_.CodeActionKind.md)  }[]

Static documentation for a class of code actions.

Documentation from the provider is shown in the code actions menu if either:

- Code actions of `kind` are requested by the editor. In this case, the editor will show the documentation that
  most closely matches the requested code action kind. For example, if a provider has documentation for
  both `Refactor` and `RefactorExtract`, when the user requests code actions for `RefactorExtract`,
  the editor will use the documentation for `RefactorExtract` instead of the documentation for `Refactor`.

- Any code actions of `kind` are returned by the provider.

At most one documentation entry will be shown per provider.

#### Defined in

[index.d.ts:2549](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2549)

___

### providedCodeActionKinds

• `Optional` `Readonly` **providedCodeActionKinds**: readonly [`CodeActionKind`](../classes/codearts_plugin_.CodeActionKind.md)[]

List of [CodeActionKinds](../classes/codearts_plugin_.CodeActionKind.md) that a [CodeActionProvider](codearts_plugin_.CodeActionProvider.md) may return.

This list is used to determine if a given `CodeActionProvider` should be invoked or not.
To avoid unnecessary computation, every `CodeActionProvider` should list use `providedCodeActionKinds`. The
list of kinds may either be generic, such as `[CodeActionKind.Refactor]`, or list out every kind provided,
such as `[CodeActionKind.Refactor.Extract.append('function'), CodeActionKind.Refactor.Extract.append('constant'), ...]`.

#### Defined in

[index.d.ts:2533](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2533)
