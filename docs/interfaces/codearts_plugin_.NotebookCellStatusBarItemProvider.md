[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookCellStatusBarItemProvider

# Interface: NotebookCellStatusBarItemProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookCellStatusBarItemProvider

A provider that can contribute items to the status bar that appears below a cell's editor.

## Table of contents

### Properties

- [onDidChangeCellStatusBarItems](codearts_plugin_.NotebookCellStatusBarItemProvider.md#ondidchangecellstatusbaritems)

### Methods

- [provideCellStatusBarItems](codearts_plugin_.NotebookCellStatusBarItemProvider.md#providecellstatusbaritems)

## Properties

### onDidChangeCellStatusBarItems

• `Optional` **onDidChangeCellStatusBarItems**: [`Event`](codearts_plugin_.Event.md)<`void`\>

An optional event to signal that statusbar items have changed. The provide method will be called again.

#### Defined in

[index.d.ts:13789](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13789)

## Methods

### provideCellStatusBarItems

▸ **provideCellStatusBarItems**(`cell`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`NotebookCellStatusBarItem`](../classes/codearts_plugin_.NotebookCellStatusBarItem.md) \| [`NotebookCellStatusBarItem`](../classes/codearts_plugin_.NotebookCellStatusBarItem.md)[]\>

The provider will be called when the cell scrolls into view, when its content, outputs, language, or metadata change, and when it changes execution state.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cell` | [`NotebookCell`](codearts_plugin_.NotebookCell.md) | The cell for which to return items. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A token triggered if this request should be cancelled. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`NotebookCellStatusBarItem`](../classes/codearts_plugin_.NotebookCellStatusBarItem.md) \| [`NotebookCellStatusBarItem`](../classes/codearts_plugin_.NotebookCellStatusBarItem.md)[]\>

One or more [cell statusbar items](../classes/codearts_plugin_.NotebookCellStatusBarItem.md)

#### Defined in

[index.d.ts:13797](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13797)
