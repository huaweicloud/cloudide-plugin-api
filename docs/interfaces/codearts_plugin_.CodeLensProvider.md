[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CodeLensProvider

# Interface: CodeLensProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).CodeLensProvider

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CodeLens`](../classes/codearts_plugin_.CodeLens.md) = [`CodeLens`](../classes/codearts_plugin_.CodeLens.md) |

## Table of contents

### Properties

- [onDidChangeCodeLenses](codearts_plugin_.CodeLensProvider.md#ondidchangecodelenses)

### Methods

- [provideCodeLenses](codearts_plugin_.CodeLensProvider.md#providecodelenses)
- [resolveCodeLens](codearts_plugin_.CodeLensProvider.md#resolvecodelens)

## Properties

### onDidChangeCodeLenses

• `Optional` **onDidChangeCodeLenses**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Defined in

[index.d.ts:2615](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2615)

## Methods

### provideCodeLenses

▸ **provideCodeLenses**(`document`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

#### Defined in

[index.d.ts:2627](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2627)

___

### resolveCodeLens

▸ `Optional` **resolveCodeLens**(`codeLens`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `codeLens` | `T` |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Defined in

[index.d.ts:2637](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2637)
