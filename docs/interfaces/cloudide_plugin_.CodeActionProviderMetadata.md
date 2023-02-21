[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CodeActionProviderMetadata

# Interface: CodeActionProviderMetadata

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CodeActionProviderMetadata

Metadata about the type of code actions that a [CodeActionProvider](#CodeActionProvider) providers

## Table of contents

### Properties

- [providedCodeActionKinds](cloudide_plugin_.CodeActionProviderMetadata.md#providedcodeactionkinds)

## Properties

### providedCodeActionKinds

• `Optional` `Readonly` **providedCodeActionKinds**: readonly [`CodeActionKind`](../classes/cloudide_plugin_.CodeActionKind.md)[]

[CodeActionKinds](#CodeActionKind) that this provider may return.

The list of kinds may be generic, such as `CodeActionKind.Refactor`, or the provider
may list our every specific kind they provide, such as `CodeActionKind.Refactor.Extract.append('function`)`

#### Defined in

[index.d.ts:8007](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8007)
