**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SourceControl

# Interface: SourceControl

An source control is able to provide [resource states](#SourceControlResourceState)
to the editor and interact with the editor in several source control related ways.

## Hierarchy

* **SourceControl**

## Index

### Properties

* [acceptInputCommand](_index_d_._plugin_.sourcecontrol.md#acceptinputcommand)
* [commitTemplate](_index_d_._plugin_.sourcecontrol.md#committemplate)
* [count](_index_d_._plugin_.sourcecontrol.md#count)
* [id](_index_d_._plugin_.sourcecontrol.md#id)
* [inputBox](_index_d_._plugin_.sourcecontrol.md#inputbox)
* [label](_index_d_._plugin_.sourcecontrol.md#label)
* [quickDiffProvider](_index_d_._plugin_.sourcecontrol.md#quickdiffprovider)
* [rootUri](_index_d_._plugin_.sourcecontrol.md#rooturi)
* [statusBarCommands](_index_d_._plugin_.sourcecontrol.md#statusbarcommands)

### Methods

* [createResourceGroup](_index_d_._plugin_.sourcecontrol.md#createresourcegroup)
* [dispose](_index_d_._plugin_.sourcecontrol.md#dispose)

## Properties

### acceptInputCommand

• `Optional` **acceptInputCommand**: [Command](_index_d_._plugin_.command.md)

*Defined in [index.d.ts:11473](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11473)*

Optional accept input command.

This command will be invoked when the user accepts the value
in the Source Control input.

___

### commitTemplate

• `Optional` **commitTemplate**: string

*Defined in [index.d.ts:11465](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11465)*

Optional commit template string.

The Source Control viewlet will populate the Source Control
input with this value when appropriate.

___

### count

• `Optional` **count**: number

*Defined in [index.d.ts:11452](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11452)*

The UI-visible count of [resource states](#SourceControlResourceState) of
this source control.

Equals to the total number of [resource state](#SourceControlResourceState)
of this source control, if undefined.

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:11428](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11428)*

The id of this source control.

___

### inputBox

• `Readonly` **inputBox**: [SourceControlInputBox](_index_d_._plugin_.sourcecontrolinputbox.md)

*Defined in [index.d.ts:11443](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11443)*

The [input box](#SourceControlInputBox) for this source control.

___

### label

• `Readonly` **label**: string

*Defined in [index.d.ts:11433](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11433)*

The human-readable label of this source control.

___

### quickDiffProvider

• `Optional` **quickDiffProvider**: [QuickDiffProvider](_index_d_._plugin_.quickdiffprovider.md)

*Defined in [index.d.ts:11457](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11457)*

An optional [quick diff provider](#QuickDiffProvider).

___

### rootUri

• `Readonly` **rootUri**: [Uri](../classes/_index_d_._plugin_.uri.md) \| undefined

*Defined in [index.d.ts:11438](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11438)*

The (optional) Uri of the root of this source control.

___

### statusBarCommands

• `Optional` **statusBarCommands**: [Command](_index_d_._plugin_.command.md)[]

*Defined in [index.d.ts:11480](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11480)*

Optional status bar commands.

These commands will be displayed in the editor's status bar.

## Methods

### createResourceGroup

▸ **createResourceGroup**(`id`: string, `label`: string): [SourceControlResourceGroup](_index_d_._plugin_.sourcecontrolresourcegroup.md)

*Defined in [index.d.ts:11485](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11485)*

Create a new [resource group](#SourceControlResourceGroup).

#### Parameters:

Name | Type |
------ | ------ |
`id` | string |
`label` | string |

**Returns:** [SourceControlResourceGroup](_index_d_._plugin_.sourcecontrolresourcegroup.md)

___

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:11490](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11490)*

Dispose this source control.

**Returns:** void
