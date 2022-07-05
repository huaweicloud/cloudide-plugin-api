[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CodeActionProvider

# Interface: CodeActionProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).CodeActionProvider

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CodeAction`](../classes/codearts_plugin_.CodeAction.md) = [`CodeAction`](../classes/codearts_plugin_.CodeAction.md) |

## Table of contents

### Methods

- [provideCodeActions](codearts_plugin_.CodeActionProvider.md#providecodeactions)
- [resolveCodeAction](codearts_plugin_.CodeActionProvider.md#resolvecodeaction)

## Methods

### provideCodeActions

▸ **provideCodeActions**(`document`, `range`, `context`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<([`Command`](codearts_plugin_.Command.md) \| `T`)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `range` | [`Range`](../classes/codearts_plugin_.Range.md) \| [`Selection`](../classes/codearts_plugin_.Selection.md) |  |
| `context` | [`CodeActionContext`](codearts_plugin_.CodeActionContext.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<([`Command`](codearts_plugin_.Command.md) \| `T`)[]\>

#### Defined in

[index.d.ts:2502](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2502)

___

### resolveCodeAction

▸ `Optional` **resolveCodeAction**(`codeAction`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `codeAction` | `T` |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

#### Defined in

[index.d.ts:2518](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L2518)
