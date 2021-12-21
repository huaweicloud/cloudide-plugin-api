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

*Defined in [index.d.ts:11353](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11353)*

Whether this source control resource group is hidden when it contains
no [source control resource states](#SourceControlResourceState).

___

### id

• `Readonly` **id**: string

*Defined in [index.d.ts:11342](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11342)*

The id of this source control resource group.

___

### label

•  **label**: string

*Defined in [index.d.ts:11347](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11347)*

The label of this source control resource group.

___

### resourceStates

•  **resourceStates**: [SourceControlResourceState](_index_d_._plugin_.sourcecontrolresourcestate.md)[]

*Defined in [index.d.ts:11359](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11359)*

This group's collection of
[source control resource states](#SourceControlResourceState).

## Methods

### dispose

▸ **dispose**(): void

*Defined in [index.d.ts:11364](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11364)*

Dispose this source control resource group.

**Returns:** void
