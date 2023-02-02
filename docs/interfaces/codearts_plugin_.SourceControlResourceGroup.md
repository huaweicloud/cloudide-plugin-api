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

[index.d.ts:14325](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L14325)

___

### id

• `Readonly` **id**: `string`

The id of this source control resource group.

#### Defined in

[index.d.ts:14314](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L14314)

___

### label

• **label**: `string`

The label of this source control resource group.

#### Defined in

[index.d.ts:14319](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L14319)

___

### resourceStates

• **resourceStates**: [`SourceControlResourceState`](codearts_plugin_.SourceControlResourceState.md)[]

This group's collection of
[source control resource states](codearts_plugin_.SourceControlResourceState.md).

#### Defined in

[index.d.ts:14331](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L14331)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose this source control resource group.

#### Returns

`void`

#### Defined in

[index.d.ts:14336](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L14336)
