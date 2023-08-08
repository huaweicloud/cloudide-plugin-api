[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / OnTypeFormattingEditProvider

# Interface: OnTypeFormattingEditProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).OnTypeFormattingEditProvider

The document formatting provider interface defines the contract between extensions and
the formatting-feature.

## Table of contents

### Methods

- [provideOnTypeFormattingEdits](codearts_plugin_.OnTypeFormattingEditProvider.md#provideontypeformattingedits)

## Methods

### provideOnTypeFormattingEdits

▸ **provideOnTypeFormattingEdits**(`document`, `position`, `ch`, `options`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TextEdit`](../classes/codearts_plugin_.TextEdit.md)[]\>

Provide formatting edits after a character has been typed.

The given position and character should hint to the provider
what range the position to expand to, like find the matching `{`
when `}` has been entered.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) | The position at which the command was invoked. |
| `ch` | `string` | The character that has been typed. |
| `options` | [`FormattingOptions`](codearts_plugin_.FormattingOptions.md) | Options controlling formatting. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`TextEdit`](../classes/codearts_plugin_.TextEdit.md)[]\>

A set of text edits or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:4027](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L4027)
