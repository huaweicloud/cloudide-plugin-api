[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DeclarationProvider

# Interface: DeclarationProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DeclarationProvider

The declaration provider interface defines the contract between extensions and
the go to declaration feature.

## Table of contents

### Methods

- [provideDeclaration](codearts_plugin_.DeclarationProvider.md#providedeclaration)

## Methods

### provideDeclaration

▸ **provideDeclaration**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Declaration`](../modules/_codearts_plugin_.md#declaration)\>

Provide the declaration of the symbol at the given position and document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | The position at which the command was invoked. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Declaration`](../modules/_codearts_plugin_.md#declaration)\>

A declaration or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:2731](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L2731)
