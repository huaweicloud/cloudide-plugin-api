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

[index.d.ts:13995](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13995)

___

### commitTemplate

• `Optional` **commitTemplate**: `string`

#### Defined in

[index.d.ts:13987](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13987)

___

### count

• `Optional` **count**: `number`

#### Defined in

[index.d.ts:13974](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13974)

___

### id

• `Readonly` **id**: `string`

#### Defined in

[index.d.ts:13949](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13949)

___

### inputBox

• `Readonly` **inputBox**: [`SourceControlInputBox`](codearts_plugin_.SourceControlInputBox.md)

#### Defined in

[index.d.ts:13964](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13964)

___

### label

• `Readonly` **label**: `string`

#### Defined in

[index.d.ts:13954](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13954)

___

### quickDiffProvider

• `Optional` **quickDiffProvider**: [`QuickDiffProvider`](codearts_plugin_.QuickDiffProvider.md)

#### Defined in

[index.d.ts:13979](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13979)

___

### rootUri

• `Readonly` **rootUri**: `undefined` \| [`Uri`](../classes/codearts_plugin_.Uri.md)

#### Defined in

[index.d.ts:13959](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L13959)

___

### statusBarCommands

• `Optional` **statusBarCommands**: [`Command`](codearts_plugin_.Command.md)[]

#### Defined in

[index.d.ts:14002](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14002)

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

[index.d.ts:14007](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14007)

___

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Defined in

[index.d.ts:14012](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L14012)
