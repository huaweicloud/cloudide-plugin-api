[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SourceControl

# Interface: SourceControl

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SourceControl

An source control is able to provide [resource states](#SourceControlResourceState)
to the editor and interact with the editor in several source control related ways.

## Table of contents

### Properties

- [acceptInputCommand](cloudide_plugin_.SourceControl.md#acceptinputcommand)
- [commitTemplate](cloudide_plugin_.SourceControl.md#committemplate)
- [count](cloudide_plugin_.SourceControl.md#count)
- [id](cloudide_plugin_.SourceControl.md#id)
- [inputBox](cloudide_plugin_.SourceControl.md#inputbox)
- [label](cloudide_plugin_.SourceControl.md#label)
- [quickDiffProvider](cloudide_plugin_.SourceControl.md#quickdiffprovider)
- [rootUri](cloudide_plugin_.SourceControl.md#rooturi)
- [statusBarCommands](cloudide_plugin_.SourceControl.md#statusbarcommands)

### Methods

- [createResourceGroup](cloudide_plugin_.SourceControl.md#createresourcegroup)
- [dispose](cloudide_plugin_.SourceControl.md#dispose)

## Properties

### acceptInputCommand

• `Optional` **acceptInputCommand**: [`Command`](cloudide_plugin_.Command.md)

Optional accept input command.

This command will be invoked when the user accepts the value
in the Source Control input.

#### Defined in

[index.d.ts:9521](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9521)

___

### commitTemplate

• `Optional` **commitTemplate**: `string`

Optional commit template string.

The Source Control viewlet will populate the Source Control
input with this value when appropriate.

#### Defined in

[index.d.ts:9513](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9513)

___

### count

• `Optional` **count**: `number`

The UI-visible count of [resource states](#SourceControlResourceState) of
this source control.

Equals to the total number of [resource state](#SourceControlResourceState)
of this source control, if undefined.

#### Defined in

[index.d.ts:9500](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9500)

___

### id

• `Readonly` **id**: `string`

The id of this source control.

#### Defined in

[index.d.ts:9476](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9476)

___

### inputBox

• `Readonly` **inputBox**: [`SourceControlInputBox`](cloudide_plugin_.SourceControlInputBox.md)

The [input box](#SourceControlInputBox) for this source control.

#### Defined in

[index.d.ts:9491](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9491)

___

### label

• `Readonly` **label**: `string`

The human-readable label of this source control.

#### Defined in

[index.d.ts:9481](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9481)

___

### quickDiffProvider

• `Optional` **quickDiffProvider**: [`QuickDiffProvider`](cloudide_plugin_.QuickDiffProvider.md)

An optional [quick diff provider](#QuickDiffProvider).

#### Defined in

[index.d.ts:9505](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9505)

___

### rootUri

• `Readonly` **rootUri**: `undefined` \| [`Uri`](../classes/cloudide_plugin_.Uri.md)

The (optional) Uri of the root of this source control.

#### Defined in

[index.d.ts:9486](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9486)

___

### statusBarCommands

• `Optional` **statusBarCommands**: [`Command`](cloudide_plugin_.Command.md)[]

Optional status bar commands.

These commands will be displayed in the editor's status bar.

#### Defined in

[index.d.ts:9528](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9528)

## Methods

### createResourceGroup

▸ **createResourceGroup**(`id`, `label`): [`SourceControlResourceGroup`](cloudide_plugin_.SourceControlResourceGroup.md)

Create a new [resource group](#SourceControlResourceGroup).

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `label` | `string` |

#### Returns

[`SourceControlResourceGroup`](cloudide_plugin_.SourceControlResourceGroup.md)

#### Defined in

[index.d.ts:9533](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9533)

___

### dispose

▸ **dispose**(): `void`

Dispose this source control.

#### Returns

`void`

#### Defined in

[index.d.ts:9538](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9538)
