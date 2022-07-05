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

[index.d.ts:15396](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L15396)

___

### items

• `Readonly` **items**: [`TestItemCollection`](codearts_plugin_.TestItemCollection.md)

#### Defined in

[index.d.ts:15415](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L15415)

___

### label

• **label**: `string`

#### Defined in

[index.d.ts:15401](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L15401)

___

### refreshHandler

• **refreshHandler**: `undefined` \| (`token`: [`CancellationToken`](codearts_plugin_.CancellationToken.md)) => `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:15461](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L15461)

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

[index.d.ts:15428](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L15428)

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

[index.d.ts:15496](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L15496)

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

[index.d.ts:15484](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L15484)

___

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:15502](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L15502)

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

[index.d.ts:15448](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L15448)
