[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DefinitionProvider

# Interface: DefinitionProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DefinitionProvider

The definition provider interface defines the contract between extensions and
the [go to definition](https://code.visualstudio.com/docs/editor/editingevolved#_go-to-definition)
and peek definition features.

## Table of contents

### Methods

- [provideDefinition](codearts_plugin_.DefinitionProvider.md#providedefinition)

## Methods

### provideDefinition

▸ **provideDefinition**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Definition`](../modules/_codearts_plugin_.md#definition) \| [`LocationLink`](codearts_plugin_.LocationLink.md)[]\>

Provide the definition of the symbol at the given position and document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | The position at which the command was invoked. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Definition`](../modules/_codearts_plugin_.md#definition) \| [`LocationLink`](codearts_plugin_.LocationLink.md)[]\>

A definition or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:2671](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L2671)
