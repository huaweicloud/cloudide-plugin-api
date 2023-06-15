[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / scm

# Namespace: scm

["@codearts/plugin"](_codearts_plugin_.md).scm

## Table of contents

### Variables

- [inputBox](codearts_plugin_.scm.md#inputbox)

### Functions

- [createSourceControl](codearts_plugin_.scm.md#createsourcecontrol)

## Variables

### inputBox

• `Const` **inputBox**: [`SourceControlInputBox`](../interfaces/codearts_plugin_.SourceControlInputBox.md)

The [input box](../interfaces/codearts_plugin_.SourceControlInputBox.md) for the last source control
created by the extension.

**`Deprecated`**

Use SourceControl.inputBox instead

#### Defined in

[index.d.ts:14860](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14860)

## Functions

### createSourceControl

▸ **createSourceControl**(`id`, `label`, `rootUri?`): [`SourceControl`](../interfaces/codearts_plugin_.SourceControl.md)

Creates a new [source control](../interfaces/codearts_plugin_.SourceControl.md) instance.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | An `id` for the source control. Something short, e.g.: `git`. |
| `label` | `string` | A human-readable string for the source control. E.g.: `Git`. |
| `rootUri?` | [`Uri`](../classes/codearts_plugin_.Uri.md) | An optional Uri of the root of the source control. E.g.: `Uri.parse(workspaceRoot)`. |

#### Returns

[`SourceControl`](../interfaces/codearts_plugin_.SourceControl.md)

An instance of [source control](../interfaces/codearts_plugin_.SourceControl.md).

#### Defined in

[index.d.ts:14870](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14870)
