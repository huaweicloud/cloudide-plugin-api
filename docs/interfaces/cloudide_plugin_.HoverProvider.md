[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / HoverProvider

# Interface: HoverProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).HoverProvider

The hover provider interface defines the contract between extensions and
the [hover](https://code.visualstudio.com/docs/editor/intellisense)-feature.

## Table of contents

### Methods

- [provideHover](cloudide_plugin_.HoverProvider.md#providehover)

## Methods

### provideHover

▸ **provideHover**(`document`, `position`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`Hover`](../classes/cloudide_plugin_.Hover.md)\>

Provide a hover for the given position and document. Multiple hovers at the same
position will be merged by the editor. A hover can have a range which defaults
to the word range at the position when omitted.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/cloudide_plugin_.Position.md) | The position at which the command was invoked. |
| `token` | `undefined` \| [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<[`Hover`](../classes/cloudide_plugin_.Hover.md)\>

A hover or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:9244](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9244)
