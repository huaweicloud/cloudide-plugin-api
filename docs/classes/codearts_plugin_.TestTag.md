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

[index.d.ts:15789](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15789)

## Properties

### id

• `Readonly` **id**: `string`

ID of the test tag. `TestTag` instances with the same ID are considered
to be identical.

#### Defined in

[index.d.ts:15783](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L15783)
