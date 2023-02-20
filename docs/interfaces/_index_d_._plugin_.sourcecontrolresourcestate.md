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
* [contextValue](_index_d_._plugin_.sourcecontrolresourcestate.md#contextvalue)
* [decorations](_index_d_._plugin_.sourcecontrolresourcestate.md#decorations)
* [resourceUri](_index_d_._plugin_.sourcecontrolresourcestate.md#resourceuri)

## Properties

### command

• `Optional` `Readonly` **command**: [Command](_index_d_._plugin_.command.md)

*Defined in [index.d.ts:11356](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11356)*

The [command](#Command) which should be run when the resource
state is open in the Source Control viewlet.

___

### contextValue

• `Optional` `Readonly` **contextValue**: string

*Defined in [index.d.ts:11382](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11382)*

Context value of the resource state. This can be used to contribute resource specific actions.
For example, if a resource is given a context value as `diffable`. When contributing actions to `scm/resourceState/context`
using `menus` extension point, you can specify context value for key `scmResourceState` in `when` expressions, like `scmResourceState == diffable`.
```
	"contributes": {
		"menus": {
			"scm/resourceState/context": [
				{
					"command": "extension.diff",
					"when": "scmResourceState == diffable"
				}
			]
		}
	}
```
This will show action `extension.diff` only for resources with `contextValue` is `diffable`.

___

### decorations

• `Optional` `Readonly` **decorations**: [SourceControlResourceDecorations](_index_d_._plugin_.sourcecontrolresourcedecorations.md)

*Defined in [index.d.ts:11362](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11362)*

The [decorations](#SourceControlResourceDecorations) for this source control
resource state.

___

### resourceUri

• `Readonly` **resourceUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:11350](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11350)*

The [uri](#Uri) of the underlying resource inside the workspace.
