**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SourceControlResourceGroup

# Interface: SourceControlResourceGroup

A source control resource group is a collection of
[source control resource states](#SourceControlResourceState).

## Hierarchy

* **SourceControlResourceGroup**

## Index

### Properties

* [hideWhenEmpty](_index_d_._plugin_.sourcecontrolresourcegroup.md#hidewhenempty)
* [id](_index_d_._plugin_.sourcecontrolresourcegroup.md#id)
* [label](_index_d_._plugin_.sourcecontrolresourcegroup.md#label)
* [resourceStates](_index_d_._plugin_.sourcecontrolresourcegroup.md#resourcestates)

### Methods

* [dispose](_index_d_._plugin_.sourcecontrolresourcegroup.md#dispose)

## Properties

### hideWhenEmpty

• `Optional` **hideWhenEmpty**: boolean

*Defined in [index.d.ts:11385](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11385)*

Whether this source control resource group is hidden when it contains
no [source control resource states](#SourceControlResourceState).

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:11374](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11374)*

The id of this source control resource group.

___

### label

•  **label**: string

*Defined in [index.d.ts:11379](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11379)*

The label of this source control resource group.

___

### resourceStates

•  **resourceStates**: [SourceControlResourceState](_index_d_._plugin_.sourcecontrolresourcestate.md)[]

*Defined in [index.d.ts:11391](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11391)*

This group's collection of
[source control resource states](#SourceControlResourceState).

## Methods

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:11396](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11396)*

Dispose this source control resource group.

**Returns:** void
