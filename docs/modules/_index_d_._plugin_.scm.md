**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](_index_d_.md) / ["plugin"](_index_d_._plugin_.md) / scm

# Namespace: scm

## Index

### Variables

* [inputBox](_index_d_._plugin_.scm.md#inputbox)

### Functions

* [createSourceControl](_index_d_._plugin_.scm.md#createsourcecontrol)

## Variables

### inputBox

• `Const` **inputBox**: [SourceControlInputBox](../interfaces/_index_d_._plugin_.sourcecontrolinputbox.md)

*Defined in [index.d.ts:11501](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11501)*

The [input box](#SourceControlInputBox) for the last source control
created by the extension.

**`deprecated`** Use SourceControl.inputBox instead

## Functions

### createSourceControl

▸ **createSourceControl**(`id`: string, `label`: string, `rootUri?`: [Uri](../classes/_index_d_._plugin_.uri.md)): [SourceControl](../interfaces/_index_d_._plugin_.sourcecontrol.md)

*Defined in [index.d.ts:11511](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11511)*

Creates a new [source control](#SourceControl) instance.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | An `id` for the source control. Something short, e.g.: `git`. |
`label` | string | A human-readable string for the source control. E.g.: `Git`. |
`rootUri?` | [Uri](../classes/_index_d_._plugin_.uri.md) | An optional Uri of the root of the source control. E.g.: `Uri.parse(workspaceRoot)`. |

**Returns:** [SourceControl](../interfaces/_index_d_._plugin_.sourcecontrol.md)

An instance of [source control](#SourceControl).
