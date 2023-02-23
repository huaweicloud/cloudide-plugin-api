[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ReferenceProvider

# Interface: ReferenceProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ReferenceProvider

The reference provider interface defines the contract between extensions and
the [find references](https://code.visualstudio.com/docs/editor/editingevolved#_peek)-feature.

## Table of contents

### Methods

- [provideReferences](cloudide_plugin_.ReferenceProvider.md#providereferences)

## Methods

### provideReferences

▸ **provideReferences**(`document`, `position`, `context`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`Location`](../classes/cloudide_plugin_.Location.md)[]\>

Provide a set of project-wide references for the given position and document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/cloudide_plugin_.Position.md) | The position at which the command was invoked. |
| `context` | [`ReferenceContext`](cloudide_plugin_.ReferenceContext.md) |  |
| `token` | [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`Location`](../classes/cloudide_plugin_.Location.md)[]\>

An array of locations or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:7338](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7338)
