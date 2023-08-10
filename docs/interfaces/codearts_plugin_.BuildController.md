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
- [executableTerminal](codearts_plugin_.BuildController.md#executableterminal)
- [openBuildOutput](codearts_plugin_.BuildController.md#openbuildoutput)
- [showBuildMessageItems](codearts_plugin_.BuildController.md#showbuildmessageitems)
- [updateBuildData](codearts_plugin_.BuildController.md#updatebuilddata)

## Properties

### id

• `Readonly` **id**: `string`

#### Defined in

[index.d.ts:16942](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16942)

___

### label

• **label**: `string`

Human-readable label for the build controller.

#### Defined in

[index.d.ts:16947](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16947)

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

[index.d.ts:16969](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16969)

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

[index.d.ts:16959](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16959)

___

### dispose

▸ **dispose**(): `void`

Unregisters the build controller, disposing of its associated builds
and unpersisted results.

#### Returns

`void`

#### Defined in

[index.d.ts:16994](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16994)

___

### executableTerminal

▸ **executableTerminal**(`cmd`, `initialText?`): `void`

executable terminal with shell in build output.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cmd` | `string` | an executable script command. |
| `initialText?` | `string` | Initial output displayed when running cmd. |

#### Returns

`void`

#### Defined in

[index.d.ts:16981](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16981)

___

### openBuildOutput

▸ **openBuildOutput**(): `void`

open build view output.

#### Returns

`void`

#### Defined in

[index.d.ts:16964](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16964)

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

[index.d.ts:16974](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16974)

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

[index.d.ts:16988](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16988)
