**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / FileDecorationProvider

# Interface: FileDecorationProvider

The decoration provider interfaces defines the contract between extensions and
file decorations.

## Hierarchy

* **FileDecorationProvider**

## Index

### Properties

* [onDidChangeFileDecorations](_index_d_._plugin_.filedecorationprovider.md#ondidchangefiledecorations)

### Methods

* [provideFileDecoration](_index_d_._plugin_.filedecorationprovider.md#providefiledecoration)

## Properties

### onDidChangeFileDecorations

• `Optional` **onDidChangeFileDecorations**: [Event](_index_d_._plugin_.event.md)\<undefined \| [Uri](../classes/_index_d_._plugin_.uri.md) \| [Uri](../classes/_index_d_._plugin_.uri.md)[]>

*Defined in [index.d.ts:5790](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5790)*

An optional event to signal that decorations for one or many files have changed.

*Note* that this event should be used to propagate information about children.

**`see`** [EventEmitter](#EventEmitter)

## Methods

### provideFileDecoration

▸ **provideFileDecoration**(`uri`: [Uri](../classes/_index_d_._plugin_.uri.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[FileDecoration](../classes/_index_d_._plugin_.filedecoration.md)>

*Defined in [index.d.ts:5803](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L5803)*

Provide decorations for a given uri.

*Note* that this function is only called when a file gets rendered in the UI.
This means a decoration from a descendent that propagates upwards must be signaled
to the editor via the [onDidChangeFileDecorations](#FileDecorationProvider.onDidChangeFileDecorations)-event.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`uri` | [Uri](../classes/_index_d_._plugin_.uri.md) | The uri of the file to provide a decoration for. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<[FileDecoration](../classes/_index_d_._plugin_.filedecoration.md)>

A decoration or a thenable that resolves to such.
