[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / tests

# Namespace: tests

["@codearts/plugin"](_codearts_plugin_.md).tests

Namespace for testing functionality. Tests are published by registering
[TestController](../interfaces/codearts_plugin_.TestController.md) instances, then adding [TestItems](../interfaces/codearts_plugin_.TestItem.md).
Controllers may also describe how to run tests by creating one or more
[TestRunProfile](../interfaces/codearts_plugin_.TestRunProfile.md) instances.

## Table of contents

### Functions

- [createTestController](codearts_plugin_.tests.md#createtestcontroller)

## Functions

### createTestController

▸ **createTestController**(`id`, `label`): [`TestController`](../interfaces/codearts_plugin_.TestController.md)

Creates a new test controller.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | Identifier for the controller, must be globally unique. |
| `label` | `string` | A human-readable label for the controller. |

#### Returns

[`TestController`](../interfaces/codearts_plugin_.TestController.md)

An instance of the [TestController](../interfaces/codearts_plugin_.TestController.md).

#### Defined in

[index.d.ts:16324](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L16324)
