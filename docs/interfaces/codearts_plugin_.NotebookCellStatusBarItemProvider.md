[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / NotebookCellStatusBarItemProvider

# Interface: NotebookCellStatusBarItemProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).NotebookCellStatusBarItemProvider

## Table of contents

### Properties

- [onDidChangeCellStatusBarItems](codearts_plugin_.NotebookCellStatusBarItemProvider.md#ondidchangecellstatusbaritems)

### Methods

- [provideCellStatusBarItems](codearts_plugin_.NotebookCellStatusBarItemProvider.md#providecellstatusbaritems)

## Properties

### onDidChangeCellStatusBarItems

• `Optional` **onDidChangeCellStatusBarItems**: [`Event`](codearts_plugin_.Event.md)<`void`\>

#### Defined in

[index.d.ts:13727](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13727)

## Methods

### provideCellStatusBarItems

▸ **provideCellStatusBarItems**(`cell`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`NotebookCellStatusBarItem`](../classes/codearts_plugin_.NotebookCellStatusBarItem.md) \| [`NotebookCellStatusBarItem`](../classes/codearts_plugin_.NotebookCellStatusBarItem.md)[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cell` | [`NotebookCell`](codearts_plugin_.NotebookCell.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`NotebookCellStatusBarItem`](../classes/codearts_plugin_.NotebookCellStatusBarItem.md) \| [`NotebookCellStatusBarItem`](../classes/codearts_plugin_.NotebookCellStatusBarItem.md)[]\>

#### Defined in

[index.d.ts:13735](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13735)
