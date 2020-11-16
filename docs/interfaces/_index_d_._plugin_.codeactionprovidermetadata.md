**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CodeActionProviderMetadata

# Interface: CodeActionProviderMetadata

Metadata about the type of code actions that a [CodeActionProvider](#CodeActionProvider) providers.

## Hierarchy

* **CodeActionProviderMetadata**

## Index

### Properties

* [providedCodeActionKinds](_index_d_._plugin_.codeactionprovidermetadata.md#providedcodeactionkinds)

## Properties

### providedCodeActionKinds

• `Optional` `Readonly` **providedCodeActionKinds**: ReadonlyArray\<[CodeActionKind](../classes/_index_d_._plugin_.codeactionkind.md)>

*Defined in [index.d.ts:2238](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2238)*

List of [CodeActionKinds](#CodeActionKind) that a [CodeActionProvider](#CodeActionProvider) may return.

This list is used to determine if a given `CodeActionProvider` should be invoked or not.
To avoid unnecessary computation, every `CodeActionProvider` should list use `providedCodeActionKinds`. The
list of kinds may either be generic, such as `[CodeActionKind.Refactor]`, or list out every kind provided,
such as `[CodeActionKind.Refactor.Extract.append('function'), CodeActionKind.Refactor.Extract.append('constant'), ...]`.
