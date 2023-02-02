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

[index.d.ts:4600](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L4600)

___

### text

• `Readonly` **text**: `string`

The text the range will be replaced with if this completion is accepted.

#### Defined in

[index.d.ts:4605](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L4605)
