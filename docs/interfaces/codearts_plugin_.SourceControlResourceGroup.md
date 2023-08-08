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

[index.d.ts:14866](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14866)

___

### id

• `Readonly` **id**: `string`

The id of this source control resource group.

#### Defined in

[index.d.ts:14855](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14855)

___

### label

• **label**: `string`

The label of this source control resource group.

#### Defined in

[index.d.ts:14860](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14860)

___

### resourceStates

• **resourceStates**: [`SourceControlResourceState`](codearts_plugin_.SourceControlResourceState.md)[]

This group's collection of
[source control resource states](codearts_plugin_.SourceControlResourceState.md).

#### Defined in

[index.d.ts:14872](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14872)

## Methods

### dispose

▸ **dispose**(): `void`

Dispose this source control resource group.

#### Returns

`void`

#### Defined in

[index.d.ts:14877](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14877)
