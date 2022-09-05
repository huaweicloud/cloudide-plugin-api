[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SourceControlResourceGroup

# Interface: SourceControlResourceGroup

["@codearts/plugin"](../modules/_codearts_plugin_.md).SourceControlResourceGroup

A source control resource group is a collection of
[source control resource states](codearts_plugin_.SourceControlResourceState.md).

## Table of contents

### Properties

- [hideWhenEmpty](codearts_plugin_.SourceControlResourceGroup.md#hidewhenempty)
- [id](codearts_plugin_.SourceControlResourceGroup.md#id)
- [label](codearts_plugin_.SourceControlResourceGroup.md#label)
- [resourceStates](codearts_plugin_.SourceControlResourceGroup.md#resourcestates)

### Methods

- [dispose](codearts_plugin_.SourceControlResourceGroup.md#dispose)

## Properties

### hideWhenEmpty

• `Optional` **hideWhenEmpty**: `boolean`

Whether this source control resource group is hidden when it contains
no [source control resource states](codearts_plugin_.SourceControlResourceState.md).

#### Defined in

[index.d.ts:13988](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13988)

___

### id

• `Readonly` **id**: `string`

The id of this source control resource group.

#### Defined in

[index.d.ts:13977](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13977)

___

### label

• **label**: `string`

The label of this source control resource group.

#### Defined in

[index.d.ts:13982](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13982)

___

### resourceStates

• **resourceStates**: [`SourceControlResourceState`](codearts_plugin_.SourceControlResourceState.md)[]

This group's collection of
[source control resource states](codearts_plugin_.SourceControlResourceState.md).

#### Defined in

[index.d.ts:13994](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13994)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose this source control resource group.

#### Returns

`void`

#### Defined in

[index.d.ts:13999](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L13999)
