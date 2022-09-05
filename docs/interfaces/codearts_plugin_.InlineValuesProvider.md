[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlineValuesProvider

# Interface: InlineValuesProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlineValuesProvider

The inline values provider interface defines the contract between extensions and the editor's debugger inline values feature.
In this contract the provider returns inline value information for a given document range
and the editor shows this information in the editor at the end of lines.

## Table of contents

### Properties

- [onDidChangeInlineValues](codearts_plugin_.InlineValuesProvider.md#ondidchangeinlinevalues)

### Methods

- [provideInlineValues](codearts_plugin_.InlineValuesProvider.md#provideinlinevalues)

## Properties

### onDidChangeInlineValues

• `Optional` **onDidChangeInlineValues**: [`Event`](codearts_plugin_.Event.md)<`void`\>

An optional event to signal that inline values have changed.

**`See`**

[EventEmitter](../classes/codearts_plugin_.EventEmitter.md)

#### Defined in

[index.d.ts:3037](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L3037)

## Methods

### provideInlineValues

▸ **provideInlineValues**(`document`, `viewPort`, `context`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`InlineValue`](../modules/_codearts_plugin_.md#inlinevalue)[]\>

Provide "inline value" information for a given document and range.
The editor calls this method whenever debugging stops in the given document.
The returned inline values information is rendered in the editor at the end of lines.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document for which the inline values information is needed. |
| `viewPort` | [`Range`](../classes/codearts_plugin_.Range.md) | The visible document range for which inline values should be computed. |
| `context` | [`InlineValueContext`](codearts_plugin_.InlineValueContext.md) | A bag containing contextual information like the current location. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`InlineValue`](../modules/_codearts_plugin_.md#inlinevalue)[]\>

An array of InlineValueDescriptors or a thenable that resolves to such. The lack of a result can be
signaled by returning `undefined` or `null`.

#### Defined in

[index.d.ts:3051](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L3051)
