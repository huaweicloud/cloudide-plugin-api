[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SourceControl

# Interface: SourceControl

["@codearts/plugin"](../modules/_codearts_plugin_.md).SourceControl

## Table of contents

### Properties

- [acceptInputCommand](codearts_plugin_.SourceControl.md#acceptinputcommand)
- [commitTemplate](codearts_plugin_.SourceControl.md#committemplate)
- [count](codearts_plugin_.SourceControl.md#count)
- [id](codearts_plugin_.SourceControl.md#id)
- [inputBox](codearts_plugin_.SourceControl.md#inputbox)
- [label](codearts_plugin_.SourceControl.md#label)
- [quickDiffProvider](codearts_plugin_.SourceControl.md#quickdiffprovider)
- [rootUri](codearts_plugin_.SourceControl.md#rooturi)
- [statusBarCommands](codearts_plugin_.SourceControl.md#statusbarcommands)

### Methods

- [createResourceGroup](codearts_plugin_.SourceControl.md#createresourcegroup)
- [dispose](codearts_plugin_.SourceControl.md#dispose)

## Properties

### acceptInputCommand

• `Optional` **acceptInputCommand**: [`Command`](codearts_plugin_.Command.md)

#### Defined in

[index.d.ts:13965](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L13965)

___

### commitTemplate

• `Optional` **commitTemplate**: `string`

#### Defined in

[index.d.ts:13957](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L13957)

___

### count

• `Optional` **count**: `number`

#### Defined in

[index.d.ts:13944](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L13944)

___

### id

• `Readonly` **id**: `string`

#### Defined in

[index.d.ts:13919](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L13919)

___

### inputBox

• `Readonly` **inputBox**: [`SourceControlInputBox`](codearts_plugin_.SourceControlInputBox.md)

#### Defined in

[index.d.ts:13934](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L13934)

___

### label

• `Readonly` **label**: `string`

#### Defined in

[index.d.ts:13924](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L13924)

___

### quickDiffProvider

• `Optional` **quickDiffProvider**: [`QuickDiffProvider`](codearts_plugin_.QuickDiffProvider.md)

#### Defined in

[index.d.ts:13949](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L13949)

___

### rootUri

• `Readonly` **rootUri**: `undefined` \| [`Uri`](../classes/codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:13929](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L13929)

___

### statusBarCommands

• `Optional` **statusBarCommands**: [`Command`](codearts_plugin_.Command.md)[]

#### Defined in

[index.d.ts:13972](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L13972)

## Methods

### createResourceGroup

▸ **createResourceGroup**(`id`, `label`): [`SourceControlResourceGroup`](codearts_plugin_.SourceControlResourceGroup.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `label` | `string` |

#### Returns

[`SourceControlResourceGroup`](codearts_plugin_.SourceControlResourceGroup.md)

#### Defined in

[index.d.ts:13977](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L13977)

___

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:13982](https://github.com/huaweicloud/cloudide-plugin-api/blob/b58031b/index.d.ts#L13982)
