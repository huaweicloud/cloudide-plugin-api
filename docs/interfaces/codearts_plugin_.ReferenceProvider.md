[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ReferenceProvider

# Interface: ReferenceProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).ReferenceProvider

## Table of contents

### Methods

- [provideReferences](codearts_plugin_.ReferenceProvider.md#providereferences)

## Methods

### provideReferences

▸ **provideReferences**(`document`, `position`, `context`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Location`](../classes/codearts_plugin_.Location.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `context` | [`ReferenceContext`](codearts_plugin_.ReferenceContext.md) | - |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Location`](../classes/codearts_plugin_.Location.md)[]\>

#### Defined in

[index.d.ts:3368](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L3368)
