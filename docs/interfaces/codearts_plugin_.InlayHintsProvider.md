[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlayHintsProvider

# Interface: InlayHintsProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlayHintsProvider

The inlay hints provider interface defines the contract between extensions and
the inlay hints feature.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`InlayHint`](../classes/codearts_plugin_.InlayHint.md) = [`InlayHint`](../classes/codearts_plugin_.InlayHint.md) |

## Table of contents

### Properties

- [onDidChangeInlayHints](codearts_plugin_.InlayHintsProvider.md#ondidchangeinlayhints)

### Methods

- [provideInlayHints](codearts_plugin_.InlayHintsProvider.md#provideinlayhints)
- [resolveInlayHint](codearts_plugin_.InlayHintsProvider.md#resolveinlayhint)

## Properties

### onDidChangeInlayHints

• `Optional` **onDidChangeInlayHints**: [`Event`](codearts_plugin_.Event.md)<`void`\>

An optional event to signal that inlay hints from this provider have changed.

#### Defined in

[index.d.ts:5038](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5038)

## Methods

### provideInlayHints

▸ **provideInlayHints**(`document`, `range`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

Provide inlay hints for the given range and document.

*Note* that inlay hints that are not [contained](../classes/codearts_plugin_.Range.md#contains) by the given range are ignored.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `range` | [`Range`](../classes/codearts_plugin_.Range.md) | The range for which inlay hints should be computed. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`[]\>

An array of inlay hints or a thenable that resolves to such.

#### Defined in

[index.d.ts:5050](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5050)

___

### resolveInlayHint

▸ `Optional` **resolveInlayHint**(`hint`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

Given an inlay hint fill in [tooltip](../classes/codearts_plugin_.InlayHint.md#tooltip), [text edits](../classes/codearts_plugin_.InlayHint.md#textedits),
or complete label [parts](../classes/codearts_plugin_.InlayHintLabelPart.md).

*Note* that the editor will resolve an inlay hint at most once.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hint` | `T` | An inlay hint. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

The resolved inlay hint or a thenable that resolves to such. It is OK to return the given `item`. When no result is returned, the given `item` will be used.

#### Defined in

[index.d.ts:5062](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5062)
