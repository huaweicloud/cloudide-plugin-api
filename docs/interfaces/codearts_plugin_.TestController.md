[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TestController

# Interface: TestController

["@codearts/plugin"](../modules/_codearts_plugin_.md).TestController

## Table of contents

### Properties

- [id](codearts_plugin_.TestController.md#id)
- [items](codearts_plugin_.TestController.md#items)
- [label](codearts_plugin_.TestController.md#label)
- [refreshHandler](codearts_plugin_.TestController.md#refreshhandler)

### Methods

- [createRunProfile](codearts_plugin_.TestController.md#createrunprofile)
- [createTestItem](codearts_plugin_.TestController.md#createtestitem)
- [createTestRun](codearts_plugin_.TestController.md#createtestrun)
- [dispose](codearts_plugin_.TestController.md#dispose)
- [resolveHandler](codearts_plugin_.TestController.md#resolvehandler)

## Properties

### id

• `Readonly` **id**: `string`

#### Defined in

[index.d.ts:15426](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15426)

___

### items

• `Readonly` **items**: [`TestItemCollection`](codearts_plugin_.TestItemCollection.md)

#### Defined in

[index.d.ts:15445](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15445)

___

### label

• **label**: `string`

#### Defined in

[index.d.ts:15431](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15431)

___

### refreshHandler

• **refreshHandler**: `undefined` \| (`token`: [`CancellationToken`](codearts_plugin_.CancellationToken.md)) => `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:15491](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15491)

## Methods

### createRunProfile

▸ **createRunProfile**(`label`, `kind`, `runHandler`, `isDefault?`, `tag?`): [`TestRunProfile`](codearts_plugin_.TestRunProfile.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `label` | `string` |  |
| `kind` | [`TestRunProfileKind`](../enums/codearts_plugin_.TestRunProfileKind.md) |  |
| `runHandler` | (`request`: [`TestRunRequest`](../classes/codearts_plugin_.TestRunRequest.md), `token`: [`CancellationToken`](codearts_plugin_.CancellationToken.md)) => `void` \| [`Thenable`](Thenable.md)<`void`\> |  |
| `isDefault?` | `boolean` |  |
| `tag?` | [`TestTag`](../classes/codearts_plugin_.TestTag.md) |  |

#### Returns

[`TestRunProfile`](codearts_plugin_.TestRunProfile.md)

#### Defined in

[index.d.ts:15458](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15458)

___

### createTestItem

▸ **createTestItem**(`id`, `label`, `uri?`): [`TestItem`](codearts_plugin_.TestItem.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` |  |
| `label` | `string` |  |
| `uri?` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

[`TestItem`](codearts_plugin_.TestItem.md)

#### Defined in

[index.d.ts:15526](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15526)

___

### createTestRun

▸ **createTestRun**(`request`, `name?`, `persist?`): [`TestRun`](codearts_plugin_.TestRun.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `request` | [`TestRunRequest`](../classes/codearts_plugin_.TestRunRequest.md) |  |
| `name?` | `string` |  |
| `persist?` | `boolean` |  |

#### Returns

[`TestRun`](codearts_plugin_.TestRun.md)

#### Defined in

[index.d.ts:15514](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15514)

___

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:15532](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15532)

___

### resolveHandler

▸ `Optional` **resolveHandler**(`item`): `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | `undefined` \| [`TestItem`](codearts_plugin_.TestItem.md) |  |

#### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:15478](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L15478)
