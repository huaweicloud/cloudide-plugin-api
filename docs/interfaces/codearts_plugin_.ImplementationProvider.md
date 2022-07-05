[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ImplementationProvider

# Interface: ImplementationProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).ImplementationProvider

## Table of contents

### Methods

- [provideImplementation](codearts_plugin_.ImplementationProvider.md#provideimplementation)

## Methods

### provideImplementation

▸ **provideImplementation**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Definition`](../modules/_codearts_plugin_.md#definition) \| [`LocationLink`](codearts_plugin_.LocationLink.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Definition`](../modules/_codearts_plugin_.md#definition) \| [`LocationLink`](codearts_plugin_.LocationLink.md)[]\>

#### Defined in

[index.d.ts:2689](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L2689)
