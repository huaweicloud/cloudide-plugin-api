**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SourceControlResourceState

# Interface: SourceControlResourceState

An source control resource state represents the state of an underlying workspace
resource within a certain [source control group](#SourceControlResourceGroup).

## Hierarchy

* **SourceControlResourceState**

## Index

### Properties

* [command](_index_d_._plugin_.sourcecontrolresourcestate.md#command)
* [decorations](_index_d_._plugin_.sourcecontrolresourcestate.md#decorations)
* [resourceUri](_index_d_._plugin_.sourcecontrolresourcestate.md#resourceuri)

## Properties

### command

• `Optional` `Readonly` **command**: [Command](_index_d_._plugin_.command.md)

*Defined in [index.d.ts:9946](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9946)*

The [command](#Command) which should be run when the resource
state is open in the Source Control viewlet.

___

### decorations

• `Optional` `Readonly` **decorations**: [SourceControlResourceDecorations](_index_d_._plugin_.sourcecontrolresourcedecorations.md)

*Defined in [index.d.ts:9952](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9952)*

The [decorations](#SourceControlResourceDecorations) for this source control
resource state.

___

### resourceUri

• `Readonly` **resourceUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:9940](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L9940)*

The [uri](#Uri) of the underlying resource inside the workspace.
