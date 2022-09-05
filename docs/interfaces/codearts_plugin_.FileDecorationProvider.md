[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileDecorationProvider

# Interface: FileDecorationProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileDecorationProvider

The decoration provider interfaces defines the contract between extensions and
file decorations.

## Table of contents

### Properties

- [onDidChangeFileDecorations](codearts_plugin_.FileDecorationProvider.md#ondidchangefiledecorations)

### Methods

- [provideFileDecoration](codearts_plugin_.FileDecorationProvider.md#providefiledecoration)

## Properties

### onDidChangeFileDecorations

• `Optional` **onDidChangeFileDecorations**: [`Event`](codearts_plugin_.Event.md)<`undefined` \| [`Uri`](../classes/codearts_plugin_.Uri.md) \| [`Uri`](../classes/codearts_plugin_.Uri.md)[]\>

An optional event to signal that decorations for one or many files have changed.

*Note* that this event should be used to propagate information about children.

**`See`**

[EventEmitter](../classes/codearts_plugin_.EventEmitter.md)

#### Defined in

[index.d.ts:6699](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6699)

## Methods

### provideFileDecoration

▸ **provideFileDecoration**(`uri`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`FileDecoration`](../classes/codearts_plugin_.FileDecoration.md)\>

Provide decorations for a given uri.

*Note* that this function is only called when a file gets rendered in the UI.
This means a decoration from a descendent that propagates upwards must be signaled
to the editor via the [onDidChangeFileDecorations](codearts_plugin_.FileDecorationProvider.md#ondidchangefiledecorations)-event.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) | The uri of the file to provide a decoration for. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`FileDecoration`](../classes/codearts_plugin_.FileDecoration.md)\>

A decoration or a thenable that resolves to such.

#### Defined in

[index.d.ts:6712](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L6712)
