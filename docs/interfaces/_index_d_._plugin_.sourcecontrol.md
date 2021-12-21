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

*Defined in [index.d.ts:11421](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11421)*

Optional accept input command.

This command will be invoked when the user accepts the value
in the Source Control input.

___

### commitTemplate

• `Optional` **commitTemplate**: string

*Defined in [index.d.ts:11413](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11413)*

Optional commit template string.

The Source Control viewlet will populate the Source Control
input with this value when appropriate.

___

### count

• `Optional` **count**: number

*Defined in [index.d.ts:11400](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11400)*

The UI-visible count of [resource states](#SourceControlResourceState) of
this source control.

Equals to the total number of [resource state](#SourceControlResourceState)
of this source control, if undefined.

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:11376](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11376)*

The id of this source control.

___

### inputBox

• `Readonly` **inputBox**: [SourceControlInputBox](_index_d_._plugin_.sourcecontrolinputbox.md)

*Defined in [index.d.ts:11391](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11391)*

The [input box](#SourceControlInputBox) for this source control.

___

### label

• `Readonly` **label**: string

*Defined in [index.d.ts:11381](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11381)*

The human-readable label of this source control.

___

### quickDiffProvider

• `Optional` **quickDiffProvider**: [QuickDiffProvider](_index_d_._plugin_.quickdiffprovider.md)

*Defined in [index.d.ts:11405](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11405)*

An optional [quick diff provider](#QuickDiffProvider).

___

### rootUri

• `Readonly` **rootUri**: [Uri](../classes/_index_d_._plugin_.uri.md) \| undefined

*Defined in [index.d.ts:11386](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11386)*

The (optional) Uri of the root of this source control.

___

### statusBarCommands

• `Optional` **statusBarCommands**: [Command](_index_d_._plugin_.command.md)[]

*Defined in [index.d.ts:11428](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11428)*

Optional status bar commands.

These commands will be displayed in the editor's status bar.

## Methods

### createResourceGroup

▸ **createResourceGroup**(`id`: string, `label`: string): [SourceControlResourceGroup](_index_d_._plugin_.sourcecontrolresourcegroup.md)

*Defined in [index.d.ts:11433](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11433)*

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

*Defined in [index.d.ts:11438](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11438)*

Dispose this source control.

**Returns:** void
