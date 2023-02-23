[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CodeLensProvider

# Interface: CodeLensProvider<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CodeLensProvider

A code lens provider adds [commands](#Command) to source text. The commands will be shown
as dedicated horizontal lines in between the source text.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CodeLens`](../classes/cloudide_plugin_.CodeLens.md) = [`CodeLens`](../classes/cloudide_plugin_.CodeLens.md) |

## Table of contents

### Properties

- [onDidChangeCodeLenses](cloudide_plugin_.CodeLensProvider.md#ondidchangecodelenses)

### Methods

- [provideCodeLenses](cloudide_plugin_.CodeLensProvider.md#providecodelenses)
- [resolveCodeLens](cloudide_plugin_.CodeLensProvider.md#resolvecodelens)

## Properties

### onDidChangeCodeLenses

• `Optional` **onDidChangeCodeLenses**: [`Event`](cloudide_plugin_.Event.md)<`void`\>

An optional event to signal that the code lenses from this provider have changed.

#### Defined in

[index.d.ts:8054](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8054)

## Methods

### provideCodeLenses

▸ **provideCodeLenses**(`document`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`[]\>

Compute a list of [lenses](#CodeLens). This call should return as fast as possible and if
computing the commands is expensive implementors should only return code lens objects with the
range set and implement [resolve](#CodeLensProvider.resolveCodeLens).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`[]\>

An array of code lenses or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:8065](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8065)

___

### resolveCodeLens

▸ `Optional` **resolveCodeLens**(`codeLens`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`\>

This function will be called for each visible code lens, usually when scrolling and after
calls to [compute](#CodeLensProvider.provideCodeLenses)-lenses.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `codeLens` | `T` | code lens that must be resolved. |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`T`\>

The given, resolved code lens or thenable that resolves to such.

#### Defined in

[index.d.ts:8074](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8074)
