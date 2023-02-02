[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CodeLensProvider

# Interface: CodeLensProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).CodeLensProvider

A code lens provider adds [commands](codearts_plugin_.Command.md) to source text. The commands will be shown
as dedicated horizontal lines in between the source text.

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

An optional event to signal that the code lenses from this provider have changed.

#### Defined in

[index.d.ts:2615](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L2615)

## Methods

### provideCodeLenses

▸ **provideCodeLenses**(`document`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

Compute a list of [lenses](../classes/codearts_plugin_.CodeLens.md). This call should return as fast as possible and if
computing the commands is expensive implementors should only return code lens objects with the
range set and implement [resolve](codearts_plugin_.CodeLensProvider.md#resolvecodelens).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

An array of code lenses or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:2627](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L2627)

___

### resolveCodeLens

▸ `Optional` **resolveCodeLens**(`codeLens`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

This function will be called for each visible code lens, usually when scrolling and after
calls to [compute](codearts_plugin_.CodeLensProvider.md#providecodelenses)-lenses.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `codeLens` | `T` | Code lens that must be resolved. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

The given, resolved code lens or thenable that resolves to such.

#### Defined in

[index.d.ts:2637](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L2637)
