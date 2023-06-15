[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TestTag

# Class: TestTag

["@codearts/plugin"](../modules/_codearts_plugin_.md).TestTag

Tags can be associated with [TestItems](../interfaces/codearts_plugin_.TestItem.md) and
[TestRunProfiles](../interfaces/codearts_plugin_.TestRunProfile.md). A profile with a tag can only
execute tests that include that tag in their [tags](../interfaces/codearts_plugin_.TestItem.md#tags) array.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.TestTag.md#constructor)

### Properties

- [id](codearts_plugin_.TestTag.md#id)

## Constructors

### constructor

• **new TestTag**(`id`)

Creates a new TestTag instance.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | ID of the test tag. |

#### Defined in

[index.d.ts:16227](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16227)

## Properties

### id

• `Readonly` **id**: `string`

ID of the test tag. `TestTag` instances with the same ID are considered
to be identical.

#### Defined in

[index.d.ts:16221](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L16221)
