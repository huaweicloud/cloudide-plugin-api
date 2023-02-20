**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TerminalLinkProvider

# Interface: TerminalLinkProvider\<T>

A provider that enables detection and handling of links within terminals.

## Type parameters

Name | Type | Default |
------ | ------ | ------ |
`T` | [TerminalLink](_index_d_._plugin_.terminallink.md) | TerminalLink |

## Hierarchy

* **TerminalLinkProvider**

## Index

### Methods

* [handleTerminalLink](_index_d_._plugin_.terminallinkprovider.md#handleterminallink)
* [provideTerminalLinks](_index_d_._plugin_.terminallinkprovider.md#provideterminallinks)

## Methods

### handleTerminalLink

▸ **handleTerminalLink**(`link`: T): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<void>

*Defined in [index.d.ts:5717](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5717)*

Handle an activated terminal link.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`link` | T | The link to handle.  |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<void>

___

### provideTerminalLinks

▸ **provideTerminalLinks**(`context`: [TerminalLinkContext](_index_d_._plugin_.terminallinkcontext.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T[]>

*Defined in [index.d.ts:5711](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5711)*

Provide terminal links for the given context. Note that this can be called multiple times
even before previous calls resolve, make sure to not share global objects (eg. `RegExp`)
that could have problems when asynchronous usage may overlap.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`context` | [TerminalLinkContext](_index_d_._plugin_.terminallinkcontext.md) | Information about what links are being provided for. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T[]>

A list of terminal links for the given line.
