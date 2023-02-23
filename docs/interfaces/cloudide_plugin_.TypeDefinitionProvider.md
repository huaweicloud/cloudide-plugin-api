[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TypeDefinitionProvider

# Interface: TypeDefinitionProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TypeDefinitionProvider

The type definition provider defines the contract between extensions and
the go to type definition feature.

## Table of contents

### Methods

- [provideTypeDefinition](cloudide_plugin_.TypeDefinitionProvider.md#providetypedefinition)

## Methods

### provideTypeDefinition

▸ **provideTypeDefinition**(`document`, `position`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`Definition`](../modules/_cloudide_plugin_.md#definition) \| [`DefinitionLink`](cloudide_plugin_.DefinitionLink.md)[]\>

Provide the type definition of the symbol at the given position and document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/cloudide_plugin_.Position.md) | The position at which the command was invoked. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`Definition`](../modules/_cloudide_plugin_.md#definition) \| [`DefinitionLink`](cloudide_plugin_.DefinitionLink.md)[]\>

A definition or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:787](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L787)
