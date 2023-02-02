[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SourceControl

# Interface: SourceControl

["@codearts/plugin"](../modules/_codearts_plugin_.md).SourceControl

An source control is able to provide [resource states](codearts_plugin_.SourceControlResourceState.md)
to the editor and interact with the editor in several source control related ways.

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

Optional accept input command.

This command will be invoked when the user accepts the value
in the Source Control input.

#### Defined in

[index.d.ts:14780](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14780)

___

### commitTemplate

• `Optional` **commitTemplate**: `string`

Optional commit template string.

The Source Control viewlet will populate the Source Control
input with this value when appropriate.

#### Defined in

[index.d.ts:14772](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14772)

___

### count

• `Optional` **count**: `number`

The UI-visible count of [resource states](codearts_plugin_.SourceControlResourceState.md) of
this source control.

If undefined, this source control will
- display its UI-visible count as zero, and
- contribute the count of its [resource states](codearts_plugin_.SourceControlResourceState.md) to the UI-visible aggregated count for all source controls

#### Defined in

[index.d.ts:14759](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14759)

___

### id

• `Readonly` **id**: `string`

The id of this source control.

#### Defined in

[index.d.ts:14734](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14734)

___

### inputBox

• `Readonly` **inputBox**: [`SourceControlInputBox`](codearts_plugin_.SourceControlInputBox.md)

The [input box](codearts_plugin_.SourceControlInputBox.md) for this source control.

#### Defined in

[index.d.ts:14749](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14749)

___

### label

• `Readonly` **label**: `string`

The human-readable label of this source control.

#### Defined in

[index.d.ts:14739](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14739)

___

### quickDiffProvider

• `Optional` **quickDiffProvider**: [`QuickDiffProvider`](codearts_plugin_.QuickDiffProvider.md)

An optional [quick diff provider](codearts_plugin_.QuickDiffProvider.md).

#### Defined in

[index.d.ts:14764](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14764)

___

### rootUri

• `Readonly` **rootUri**: `undefined` \| [`Uri`](../classes/codearts_plugin_.Uri.md)

The (optional) Uri of the root of this source control.

#### Defined in

[index.d.ts:14744](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14744)

___

### statusBarCommands

• `Optional` **statusBarCommands**: [`Command`](codearts_plugin_.Command.md)[]

Optional status bar commands.

These commands will be displayed in the editor's status bar.

#### Defined in

[index.d.ts:14787](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14787)

## Methods

### createResourceGroup

▸ **createResourceGroup**(`id`, `label`): [`SourceControlResourceGroup`](codearts_plugin_.SourceControlResourceGroup.md)

Create a new [resource group](codearts_plugin_.SourceControlResourceGroup.md).

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `label` | `string` |

#### Returns

[`SourceControlResourceGroup`](codearts_plugin_.SourceControlResourceGroup.md)

#### Defined in

[index.d.ts:14792](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14792)

___

### dispose

▸ **dispose**(): `void`

Dispose this source control.

#### Returns

`void`

#### Defined in

[index.d.ts:14797](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14797)
