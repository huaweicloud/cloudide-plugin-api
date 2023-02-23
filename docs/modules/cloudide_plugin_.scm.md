[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](_cloudide_plugin_.md) / scm

# Namespace: scm

["@cloudide/plugin"](_cloudide_plugin_.md).scm

## Table of contents

### Variables

- [inputBox](cloudide_plugin_.scm.md#inputbox)

### Functions

- [createSourceControl](cloudide_plugin_.scm.md#createsourcecontrol)

## Variables

### inputBox

• `Const` **inputBox**: [`SourceControlInputBox`](../interfaces/cloudide_plugin_.SourceControlInputBox.md)

~~The [input box](#SourceControlInputBox) for the last source control
created by the extension.~~

**`Deprecated`**

Use SourceControl.inputBox instead

#### Defined in

[index.d.ts:9549](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9549)

## Functions

### createSourceControl

▸ **createSourceControl**(`id`, `label`, `rootUri?`): [`SourceControl`](../interfaces/cloudide_plugin_.SourceControl.md)

Creates a new [source control](#SourceControl) instance.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | An `id` for the source control. Something short, eg: `git`. |
| `label` | `string` | A human-readable string for the source control. Eg: `Git`. |
| `rootUri?` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | An optional Uri of the root of the source control. Eg: `Uri.parse(workspaceRoot)`. |

#### Returns

[`SourceControl`](../interfaces/cloudide_plugin_.SourceControl.md)

An instance of [source control](#SourceControl).

#### Defined in

[index.d.ts:9559](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9559)
