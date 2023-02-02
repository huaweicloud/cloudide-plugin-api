[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / BuildController

# Interface: BuildController

["@codearts/plugin"](../modules/_codearts_plugin_.md).BuildController

## Table of contents

### Properties

- [id](codearts_plugin_.BuildController.md#id)
- [label](codearts_plugin_.BuildController.md#label)

### Methods

- [addBuildOutputMessage](codearts_plugin_.BuildController.md#addbuildoutputmessage)
- [createBuildProfile](codearts_plugin_.BuildController.md#createbuildprofile)
- [dispose](codearts_plugin_.BuildController.md#dispose)
- [openBuildOutput](codearts_plugin_.BuildController.md#openbuildoutput)
- [showBuildMessageItems](codearts_plugin_.BuildController.md#showbuildmessageitems)
- [updateBuildData](codearts_plugin_.BuildController.md#updatebuilddata)

## Properties

### id

• `Readonly` **id**: `string`

#### Defined in

[index.d.ts:16752](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16752)

___

### label

• **label**: `string`

Human-readable label for the build controller.

#### Defined in

[index.d.ts:16757](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16757)

## Methods

### addBuildOutputMessage

▸ **addBuildOutputMessage**(`message`): `void`

add a message to build view output.

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | [`BuildMessage`](codearts_plugin_.BuildMessage.md) |

#### Returns

`void`

#### Defined in

[index.d.ts:16779](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16779)

___

### createBuildProfile

▸ **createBuildProfile**(`options`): [`BuildProfile`](codearts_plugin_.BuildProfile.md)

Creates a profile used for running builds. Extensions must create
at least one profile in order for builds to be run.

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`BuildProfileOptions`](codearts_plugin_.BuildProfileOptions.md) |

#### Returns

[`BuildProfile`](codearts_plugin_.BuildProfile.md)

An instance of a [BuildProfile](codearts_plugin_.BuildProfile.md), which is automatically
associated with this controller.

#### Defined in

[index.d.ts:16769](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16769)

___

### dispose

▸ **dispose**(): `void`

Unregisters the build controller, disposing of its associated builds
and unpersisted results.

#### Returns

`void`

#### Defined in

[index.d.ts:16797](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16797)

___

### openBuildOutput

▸ **openBuildOutput**(): `void`

open build view output.

#### Returns

`void`

#### Defined in

[index.d.ts:16774](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16774)

___

### showBuildMessageItems

▸ **showBuildMessageItems**(`message`): `void`

show build items in build view output.

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | [`BuildMessage`](codearts_plugin_.BuildMessage.md) |

#### Returns

`void`

#### Defined in

[index.d.ts:16784](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16784)

___

### updateBuildData

▸ **updateBuildData**(`data`, `onlyUpdateMessage?`): `void`

update current BuildContoller tree

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`BuildDataItem`](codearts_plugin_.BuildDataItem.md)[] |  |
| `onlyUpdateMessage?` | `boolean` | only update Build message can not refresh treeView |

#### Returns

`void`

#### Defined in

[index.d.ts:16791](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16791)
