[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SourceControlResourceState

# Interface: SourceControlResourceState

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SourceControlResourceState

An source control resource state represents the state of an underlying workspace
resource within a certain [source control group](#SourceControlResourceGroup).

## Table of contents

### Properties

- [command](cloudide_plugin_.SourceControlResourceState.md#command)
- [contextValue](cloudide_plugin_.SourceControlResourceState.md#contextvalue)
- [decorations](cloudide_plugin_.SourceControlResourceState.md#decorations)
- [resourceUri](cloudide_plugin_.SourceControlResourceState.md#resourceuri)

## Properties

### command

• `Optional` `Readonly` **command**: [`Command`](cloudide_plugin_.Command.md)

The [command](#Command) which should be run when the resource
state is open in the Source Control viewlet.

#### Defined in

[index.d.ts:9404](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9404)

___

### contextValue

• `Optional` `Readonly` **contextValue**: `string`

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

#### Defined in

[index.d.ts:9430](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9430)

___

### decorations

• `Optional` `Readonly` **decorations**: [`SourceControlResourceDecorations`](cloudide_plugin_.SourceControlResourceDecorations.md)

The [decorations](#SourceControlResourceDecorations) for this source control
resource state.

#### Defined in

[index.d.ts:9410](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9410)

___

### resourceUri

• `Readonly` **resourceUri**: [`Uri`](../classes/cloudide_plugin_.Uri.md)

The [uri](#Uri) of the underlying resource inside the workspace.

#### Defined in

[index.d.ts:9398](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9398)
