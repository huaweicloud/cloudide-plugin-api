[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / OnTypeFormattingEditProvider

# Interface: OnTypeFormattingEditProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).OnTypeFormattingEditProvider

The document formatting provider interface defines the contract between extensions and
the formatting-feature.

## Table of contents

### Methods

- [provideOnTypeFormattingEdits](cloudide_plugin_.OnTypeFormattingEditProvider.md#provideontypeformattingedits)

## Methods

### provideOnTypeFormattingEdits

▸ **provideOnTypeFormattingEdits**(`document`, `position`, `ch`, `options`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`undefined` \| [`TextEdit`](../classes/cloudide_plugin_.TextEdit.md)[]\>

Provide formatting edits after a character has been typed.

The given position and character should hint to the provider
what range the position to expand to, like find the matching `{`
when `}` has been entered.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/cloudide_plugin_.Position.md) | The position at which the command was invoked. |
| `ch` | `string` | The character that has been typed. |
| `options` | [`FormattingOptions`](cloudide_plugin_.FormattingOptions.md) | Options controlling formatting. |
| `token` | `undefined` \| [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<`undefined` \| [`TextEdit`](../classes/cloudide_plugin_.TextEdit.md)[]\>

A set of text edits or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:8431](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8431)
