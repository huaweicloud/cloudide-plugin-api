[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlineValuesProvider

# Interface: InlineValuesProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlineValuesProvider

## Table of contents

### Properties

- [onDidChangeInlineValues](codearts_plugin_.InlineValuesProvider.md#ondidchangeinlinevalues)

### Methods

- [provideInlineValues](codearts_plugin_.InlineValuesProvider.md#provideinlinevalues)

## Properties

### onDidChangeInlineValues

• `Optional` **onDidChangeInlineValues**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Defined in

[index.d.ts:3037](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L3037)

## Methods

### provideInlineValues

▸ **provideInlineValues**(`document`, `viewPort`, `context`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`InlineValue`](../modules/_codearts_plugin_.md#inlinevalue)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `viewPort` | [`Range`](../classes/codearts_plugin_.Range.md) |  |
| `context` | [`InlineValueContext`](codearts_plugin_.InlineValueContext.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`InlineValue`](../modules/_codearts_plugin_.md#inlinevalue)[]\>

#### Defined in

[index.d.ts:3051](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L3051)
