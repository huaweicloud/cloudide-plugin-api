[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DefinitionProvider

# Interface: DefinitionProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DefinitionProvider

The definition provider interface defines the contract between extensions and
the [go to definition](https://code.visualstudio.com/docs/editor/editingevolved#_go-to-definition)
and peek definition features.

## Table of contents

### Methods

- [provideDefinition](cloudide_plugin_.DefinitionProvider.md#providedefinition)

## Methods

### provideDefinition

▸ **provideDefinition**(`document`, `position`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`Definition`](../modules/_cloudide_plugin_.md#definition) \| [`DefinitionLink`](cloudide_plugin_.DefinitionLink.md)[]\>

Provide the definition of the symbol at the given position and document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/cloudide_plugin_.Position.md) | The position at which the command was invoked. |
| `token` | `undefined` \| [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`Definition`](../modules/_cloudide_plugin_.md#definition) \| [`DefinitionLink`](cloudide_plugin_.DefinitionLink.md)[]\>

A definition or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:733](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L733)
