[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SourceControlResourceGroup

# Interface: SourceControlResourceGroup

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SourceControlResourceGroup

A source control resource group is a collection of
[source control resource states](#SourceControlResourceState).

## Table of contents

### Properties

- [hideWhenEmpty](cloudide_plugin_.SourceControlResourceGroup.md#hidewhenempty)
- [id](cloudide_plugin_.SourceControlResourceGroup.md#id)
- [label](cloudide_plugin_.SourceControlResourceGroup.md#label)
- [resourceStates](cloudide_plugin_.SourceControlResourceGroup.md#resourcestates)

### Methods

- [dispose](cloudide_plugin_.SourceControlResourceGroup.md#dispose)

## Properties

### hideWhenEmpty

• `Optional` **hideWhenEmpty**: `boolean`

Whether this source control resource group is hidden when it contains
no [source control resource states](#SourceControlResourceState).

#### Defined in

[index.d.ts:9453](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9453)

___

### id

• `Readonly` **id**: `string`

The id of this source control resource group.

#### Defined in

[index.d.ts:9442](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9442)

___

### label

• **label**: `string`

The label of this source control resource group.

#### Defined in

[index.d.ts:9447](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9447)

___

### resourceStates

• **resourceStates**: [`SourceControlResourceState`](cloudide_plugin_.SourceControlResourceState.md)[]

This group's collection of
[source control resource states](#SourceControlResourceState).

#### Defined in

[index.d.ts:9459](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9459)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose this source control resource group.

#### Returns

`void`

#### Defined in

[index.d.ts:9464](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9464)
