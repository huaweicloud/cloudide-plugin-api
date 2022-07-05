[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileSystem

# Interface: FileSystem

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileSystem

## Table of contents

### Methods

- [copy](codearts_plugin_.FileSystem.md#copy)
- [createDirectory](codearts_plugin_.FileSystem.md#createdirectory)
- [delete](codearts_plugin_.FileSystem.md#delete)
- [isWritableFileSystem](codearts_plugin_.FileSystem.md#iswritablefilesystem)
- [readDirectory](codearts_plugin_.FileSystem.md#readdirectory)
- [readFile](codearts_plugin_.FileSystem.md#readfile)
- [rename](codearts_plugin_.FileSystem.md#rename)
- [stat](codearts_plugin_.FileSystem.md#stat)
- [writeFile](codearts_plugin_.FileSystem.md#writefile)

## Methods

### copy

▸ **copy**(`source`, `target`, `options?`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `target` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `options?` | `Object` |  |
| `options.overwrite?` | `boolean` | - |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8158](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L8158)

___

### createDirectory

▸ **createDirectory**(`uri`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8116](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L8116)

___

### delete

▸ **delete**(`uri`, `options?`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `options?` | `Object` |  |
| `options.recursive?` | `boolean` | - |
| `options.useTrash?` | `boolean` | - |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8140](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L8140)

___

### isWritableFileSystem

▸ **isWritableFileSystem**(`scheme`): `undefined` \| `boolean`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scheme` | `string` |  |

#### Returns

`undefined` \| `boolean`

#### Defined in

[index.d.ts:8173](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L8173)

___

### readDirectory

▸ **readDirectory**(`uri`): [`Thenable`](Thenable.md)<[`string`, [`FileType`](../enums/codearts_plugin_.FileType.md)][]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

[`Thenable`](Thenable.md)<[`string`, [`FileType`](../enums/codearts_plugin_.FileType.md)][]\>

#### Defined in

[index.d.ts:8106](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L8106)

___

### readFile

▸ **readFile**(`uri`): [`Thenable`](Thenable.md)<`Uint8Array`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

[`Thenable`](Thenable.md)<`Uint8Array`\>

#### Defined in

[index.d.ts:8124](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L8124)

___

### rename

▸ **rename**(`source`, `target`, `options?`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `target` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `options?` | `Object` |  |
| `options.overwrite?` | `boolean` | - |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8149](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L8149)

___

### stat

▸ **stat**(`uri`): [`Thenable`](Thenable.md)<[`FileStat`](codearts_plugin_.FileStat.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

[`Thenable`](Thenable.md)<[`FileStat`](codearts_plugin_.FileStat.md)\>

#### Defined in

[index.d.ts:8098](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L8098)

___

### writeFile

▸ **writeFile**(`uri`, `content`): [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uri` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |
| `content` | `Uint8Array` |  |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:8132](https://github.com/huaweicloud/cloudide-plugin-api/blob/a4193a8/index.d.ts#L8132)
