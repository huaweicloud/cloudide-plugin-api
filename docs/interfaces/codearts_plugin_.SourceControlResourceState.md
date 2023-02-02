[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SourceControlResourceState

# Interface: SourceControlResourceState

["@codearts/plugin"](../modules/_codearts_plugin_.md).SourceControlResourceState

An source control resource state represents the state of an underlying workspace
resource within a certain [source control group](codearts_plugin_.SourceControlResourceGroup.md).

## Table of contents

### Properties

- [command](codearts_plugin_.SourceControlResourceState.md#command)
- [contextValue](codearts_plugin_.SourceControlResourceState.md#contextvalue)
- [decorations](codearts_plugin_.SourceControlResourceState.md#decorations)
- [resourceUri](codearts_plugin_.SourceControlResourceState.md#resourceuri)

## Properties

### command

• `Optional` `Readonly` **command**: [`Command`](codearts_plugin_.Command.md)

The [Command](codearts_plugin_.Command.md) which should be run when the resource
state is open in the Source Control viewlet.

#### Defined in

[index.d.ts:14662](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14662)

___

### contextValue

• `Optional` `Readonly` **contextValue**: `string`

Context value of the resource state. This can be used to contribute resource specific actions.
For example, if a resource is given a context value as `diffable`. When contributing actions to `scm/resourceState/context`
using `menus` extension point, you can specify context value for key `scmResourceState` in `when` expressions, like `scmResourceState == diffable`.
```json
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

[index.d.ts:14688](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14688)

___

### decorations

• `Optional` `Readonly` **decorations**: [`SourceControlResourceDecorations`](codearts_plugin_.SourceControlResourceDecorations.md)

The [decorations](codearts_plugin_.SourceControlResourceDecorations.md) for this source control
resource state.

#### Defined in

[index.d.ts:14668](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14668)

___

### resourceUri

• `Readonly` **resourceUri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The [Uri](../classes/codearts_plugin_.Uri.md) of the underlying resource inside the workspace.

#### Defined in

[index.d.ts:14656](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14656)
