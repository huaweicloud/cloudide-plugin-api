[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileSystemProvider

# Interface: FileSystemProvider

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileSystemProvider

## Table of contents

### Properties

- [onDidChangeFile](codearts_plugin_.FileSystemProvider.md#ondidchangefile)

### Methods

- [copy](codearts_plugin_.FileSystemProvider.md#copy)
- [createDirectory](codearts_plugin_.FileSystemProvider.md#createdirectory)
- [delete](codearts_plugin_.FileSystemProvider.md#delete)
- [readDirectory](codearts_plugin_.FileSystemProvider.md#readdirectory)
- [readFile](codearts_plugin_.FileSystemProvider.md#readfile)
- [rename](codearts_plugin_.FileSystemProvider.md#rename)
- [stat](codearts_plugin_.FileSystemProvider.md#stat)
- [watch](codearts_plugin_.FileSystemProvider.md#watch)
- [writeFile](codearts_plugin_.FileSystemProvider.md#writefile)

## Properties

### onDidChangeFile

• `Readonly` **onDidChangeFile**: [`Event`](codearts_plugin_.Event.md)<[`FileChangeEvent`](codearts_plugin_.FileChangeEvent.md)[]\>

#### Defined in

[index.d.ts:7965](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L7965)

## Methods

### copy

▸ `Optional` **copy**(`source`, `destination`, `options`): `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `destination` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `options` | `Object` |  |
| `options.overwrite` | `boolean` | - |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8079](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L8079)

___

### createDirectory

▸ **createDirectory**(`uri`): `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8020](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L8020)

___

### delete

▸ **delete**(`uri`, `options`): `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `options` | `Object` |  |
| `options.recursive` | `boolean` | - |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8052](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L8052)

___

### readDirectory

▸ **readDirectory**(`uri`): [`string`, [`FileType`](../enums/codearts_plugin_.FileType.md)][] \| [`Thenable`](Thenable.md)<[`string`, [`FileType`](../enums/codearts_plugin_.FileType.md)][]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

[`string`, [`FileType`](../enums/codearts_plugin_.FileType.md)][] \| [`Thenable`](Thenable.md)<[`string`, [`FileType`](../enums/codearts_plugin_.FileType.md)][]\>

#### Defined in

[index.d.ts:8010](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L8010)

___

### readFile

▸ **readFile**(`uri`): `Uint8Array` \| [`Thenable`](Thenable.md)<`Uint8Array`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

`Uint8Array` \| [`Thenable`](Thenable.md)<`Uint8Array`\>

#### Defined in

[index.d.ts:8029](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L8029)

___

### rename

▸ **rename**(`oldUri`, `newUri`, `options`): `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldUri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `newUri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `options` | `Object` |  |
| `options.overwrite` | `boolean` | - |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8065](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L8065)

___

### stat

▸ **stat**(`uri`): [`FileStat`](codearts_plugin_.FileStat.md) \| [`Thenable`](Thenable.md)<[`FileStat`](codearts_plugin_.FileStat.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

[`FileStat`](codearts_plugin_.FileStat.md) \| [`Thenable`](Thenable.md)<[`FileStat`](codearts_plugin_.FileStat.md)\>

#### Defined in

[index.d.ts:8001](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L8001)

___

### watch

▸ **watch**(`uri`, `options`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `options` | `Object` |  |
| `options.excludes` | readonly `string`[] | - |
| `options.recursive` | `boolean` | - |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:7988](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L7988)

___

### writeFile

▸ **writeFile**(`uri`, `content`, `options`): `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `content` | `Uint8Array` |  |
| `options` | `Object` |  |
| `options.create` | `boolean` | - |
| `options.overwrite` | `boolean` | - |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8042](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L8042)
