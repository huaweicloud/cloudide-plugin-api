[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DeclarationProvider

# Interface: DeclarationProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).DeclarationProvider

## Table of contents

### Methods

- [provideDeclaration](codearts_plugin_.DeclarationProvider.md#providedeclaration)

## Methods

### provideDeclaration

▸ **provideDeclaration**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Declaration`](../modules/_codearts_plugin_.md#declaration)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Declaration`](../modules/_codearts_plugin_.md#declaration)\>

#### Defined in

[index.d.ts:2731](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2731)
