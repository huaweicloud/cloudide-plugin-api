**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / OnTypeFormattingEditProvider

# Interface: OnTypeFormattingEditProvider

The document formatting provider interface defines the contract between extensions and
the formatting-feature.

## Hierarchy

* **OnTypeFormattingEditProvider**

## Index

### Methods

* [provideOnTypeFormattingEdits](_index_d_._plugin_.ontypeformattingeditprovider.md#provideontypeformattingedits)

## Methods

### provideOnTypeFormattingEdits

▸ **provideOnTypeFormattingEdits**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `position`: [Position](../classes/_index_d_._plugin_.position.md), `ch`: string, `options`: [FormattingOptions](_index_d_._plugin_.formattingoptions.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[TextEdit](../classes/_index_d_._plugin_.textedit.md)[]>

*Defined in [index.d.ts:3720](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L3720)*

Provide formatting edits after a character has been typed.

The given position and character should hint to the provider
what range the position to expand to, like find the matching `{`
when `}` has been entered.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`position` | [Position](../classes/_index_d_._plugin_.position.md) | The position at which the command was invoked. |
`ch` | string | The character that has been typed. |
`options` | [FormattingOptions](_index_d_._plugin_.formattingoptions.md) | Options controlling formatting. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[TextEdit](../classes/_index_d_._plugin_.textedit.md)[]>

A set of text edits or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.
