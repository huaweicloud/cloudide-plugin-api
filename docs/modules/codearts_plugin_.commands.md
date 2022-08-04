[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / commands

# Namespace: commands

["@codearts/plugin"](_codearts_plugin_.md).commands

## Table of contents

### Functions

- [executeCommand](codearts_plugin_.commands.md#executecommand)
- [getCommands](codearts_plugin_.commands.md#getcommands)
- [registerCommand](codearts_plugin_.commands.md#registercommand)
- [registerTextEditorCommand](codearts_plugin_.commands.md#registertexteditorcommand)

## Functions

### executeCommand

▸ **executeCommand**<`T`\>(`command`, ...`rest`): [`Thenable`](../interfaces/Thenable.md)<`T`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `unknown` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `command` | `string` |  |
| `...rest` | `any`[] |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`T`\>

#### Defined in

[index.d.ts:9255](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9255)

___

### getCommands

▸ **getCommands**(`filterInternal?`): [`Thenable`](../interfaces/Thenable.md)<`string`[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `filterInternal?` | `boolean` |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`string`[]\>

#### Defined in

[index.d.ts:9264](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9264)

___

### registerCommand

▸ **registerCommand**(`command`, `callback`, `thisArg?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `command` | `string` |  |
| `callback` | (...`args`: `any`[]) => `any` |  |
| `thisArg?` | `any` |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9222](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9222)

___

### registerTextEditorCommand

▸ **registerTextEditorCommand**(`command`, `callback`, `thisArg?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `command` | `string` |  |
| `callback` | (`textEditor`: [`TextEditor`](../interfaces/codearts_plugin_.TextEditor.md), `edit`: [`TextEditorEdit`](../interfaces/codearts_plugin_.TextEditorEdit.md), ...`args`: `any`[]) => `void` |  |
| `thisArg?` | `any` |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:9239](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L9239)
