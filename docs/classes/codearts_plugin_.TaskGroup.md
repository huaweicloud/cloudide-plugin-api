[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TaskGroup

# Class: TaskGroup

["@codearts/plugin"](../modules/_codearts_plugin_.md).TaskGroup

A grouping for tasks. The editor by default supports the
'Clean', 'Build', 'RebuildAll' and 'Test' group.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.TaskGroup.md#constructor)

### Properties

- [id](codearts_plugin_.TaskGroup.md#id)
- [isDefault](codearts_plugin_.TaskGroup.md#isdefault)
- [Build](codearts_plugin_.TaskGroup.md#build)
- [Clean](codearts_plugin_.TaskGroup.md#clean)
- [Rebuild](codearts_plugin_.TaskGroup.md#rebuild)
- [Test](codearts_plugin_.TaskGroup.md#test)

## Constructors

### constructor

• `Private` **new TaskGroup**(`id`, `label`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `label` | `string` |

#### Defined in

[index.d.ts:7252](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7252)

## Properties

### id

• `Readonly` **id**: `string`

The ID of the task group. Is one of TaskGroup.Clean.id, TaskGroup.Build.id, TaskGroup.Rebuild.id, or TaskGroup.Test.id.

#### Defined in

[index.d.ts:7250](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7250)

___

### isDefault

• `Readonly` **isDefault**: `undefined` \| `boolean`

Whether the task that is part of this group is the default for the group.
This property cannot be set through API, and is controlled by a user's task configurations.

#### Defined in

[index.d.ts:7245](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7245)

___

### Build

▪ `Static` **Build**: [`TaskGroup`](codearts_plugin_.TaskGroup.md)

The build task group;

#### Defined in

[index.d.ts:7229](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7229)

___

### Clean

▪ `Static` **Clean**: [`TaskGroup`](codearts_plugin_.TaskGroup.md)

The clean task group;

#### Defined in

[index.d.ts:7224](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7224)

___

### Rebuild

▪ `Static` **Rebuild**: [`TaskGroup`](codearts_plugin_.TaskGroup.md)

The rebuild all task group;

#### Defined in

[index.d.ts:7234](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7234)

___

### Test

▪ `Static` **Test**: [`TaskGroup`](codearts_plugin_.TaskGroup.md)

The test all task group;

#### Defined in

[index.d.ts:7239](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L7239)
