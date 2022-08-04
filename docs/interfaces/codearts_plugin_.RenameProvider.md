[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / RenameProvider

# Interface: RenameProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).RenameProvider

## Table of contents

### Methods

- [prepareRename](codearts_plugin_.RenameProvider.md#preparerename)
- [provideRenameEdits](codearts_plugin_.RenameProvider.md#providerenameedits)

## Methods

### prepareRename

▸ `Optional` **prepareRename**(`document`, `position`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Range`](../classes/codearts_plugin_.Range.md) \| { `placeholder`: `string` ; `range`: [`Range`](../classes/codearts_plugin_.Range.md)  }\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`Range`](../classes/codearts_plugin_.Range.md) \| { `placeholder`: `string` ; `range`: [`Range`](../classes/codearts_plugin_.Range.md)  }\>

#### Defined in

[index.d.ts:3676](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L3676)

___

### provideRenameEdits

▸ **provideRenameEdits**(`document`, `position`, `newName`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`WorkspaceEdit`](../classes/codearts_plugin_.WorkspaceEdit.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) |  |
| `position` | [`Position`](../classes/codearts_plugin_.Position.md) |  |
| `newName` | `string` |  |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) |  |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<[`WorkspaceEdit`](../classes/codearts_plugin_.WorkspaceEdit.md)\>

#### Defined in

[index.d.ts:3661](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L3661)
