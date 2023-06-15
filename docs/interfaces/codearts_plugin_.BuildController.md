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

[index.d.ts:16833](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16833)

___

### label

• **label**: `string`

Human-readable label for the build controller.

#### Defined in

[index.d.ts:16838](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16838)

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

[index.d.ts:16860](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16860)

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

[index.d.ts:16850](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16850)

___

### dispose

▸ **dispose**(): `void`

Unregisters the build controller, disposing of its associated builds
and unpersisted results.

#### Returns

`void`

#### Defined in

[index.d.ts:16885](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16885)

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

[index.d.ts:16872](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16872)

___

### openBuildOutput

▸ **openBuildOutput**(): `void`

open build view output.

#### Returns

`void`

#### Defined in

[index.d.ts:16855](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16855)

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

[index.d.ts:16865](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16865)

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

[index.d.ts:16879](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16879)
