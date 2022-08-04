[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlayHintsProvider

# Interface: InlayHintsProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlayHintsProvider

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`InlayHint`](../classes/codearts_plugin_.InlayHint.md) = [`InlayHint`](../classes/codearts_plugin_.InlayHint.md) |

## Table of contents

### Properties

- [onDidChangeInlayHints](codearts_plugin_.InlayHintsProvider.md#ondidchangeinlayhints)

### Methods

- [provideInlayHints](codearts_plugin_.InlayHintsProvider.md#provideinlayhints)
- [resolveInlayHint](codearts_plugin_.InlayHintsProvider.md#resolveinlayhint)

## Properties

### onDidChangeInlayHints

• `Optional` **onDidChangeInlayHints**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Defined in

[index.d.ts:4980](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L4980)

## Methods

### provideInlayHints

▸ **provideInlayHints**(`document`, `range`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `range` | [`Range`](../classes/codearts_plugin_.Range.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

#### Defined in

[index.d.ts:4992](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L4992)

___

### resolveInlayHint

▸ `Optional` **resolveInlayHint**(`hint`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hint` | `T` |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Defined in

[index.d.ts:5004](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L5004)
