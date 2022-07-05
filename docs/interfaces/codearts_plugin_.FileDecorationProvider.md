[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileDecorationProvider

# Interface: FileDecorationProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileDecorationProvider

## Table of contents

### Properties

- [onDidChangeFileDecorations](codearts_plugin_.FileDecorationProvider.md#ondidchangefiledecorations)

### Methods

- [provideFileDecoration](codearts_plugin_.FileDecorationProvider.md#providefiledecoration)

## Properties

### onDidChangeFileDecorations

• `Optional` **onDidChangeFileDecorations**: [`Event`](codearts_plugin_.Event.md)<`undefined` \| [`Uri`](../classes/codearts_plugin_.Uri.md) \| [`Uri`](../classes/codearts_plugin_.Uri.md)[]\>

#### Defined in

[index.d.ts:6699](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L6699)

## Methods

### provideFileDecoration

▸ **provideFileDecoration**(`uri`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`FileDecoration`](../classes/codearts_plugin_.FileDecoration.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`FileDecoration`](../classes/codearts_plugin_.FileDecoration.md)\>

#### Defined in

[index.d.ts:6712](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L6712)
