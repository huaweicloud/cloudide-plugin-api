[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SelectedCompletionInfo

# Interface: SelectedCompletionInfo

["@codearts/plugin"](../modules/_codearts_plugin_.md).SelectedCompletionInfo

Describes the currently selected completion item.

## Table of contents

### Properties

- [range](codearts_plugin_.SelectedCompletionInfo.md#range)
- [text](codearts_plugin_.SelectedCompletionInfo.md#text)

## Properties

### range

• `Readonly` **range**: [`Range`](../classes/codearts_plugin_.Range.md)

The range that will be replaced if this completion item is accepted.

#### Defined in

[index.d.ts:4638](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L4638)

___

### text

• `Readonly` **text**: `string`

The text the range will be replaced with if this completion is accepted.

#### Defined in

[index.d.ts:4643](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L4643)
