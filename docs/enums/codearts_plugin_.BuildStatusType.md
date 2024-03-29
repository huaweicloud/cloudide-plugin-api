[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / BuildStatusType

# Enumeration: BuildStatusType

["@codearts/plugin"](../modules/_codearts_plugin_.md).BuildStatusType

Currently, there are four different states for build tasks, each with a distinct UI representation.
In the initial state, the project is in a buildable state and the build button is active while the stop button is inactive.
The starting and stopping states are the same, indicating that the project is preparing to build or ending a build, respectively.
Both of the above cases, the UI shows both the build and stop buttons as inactive.
The building state represents an active build and the UI shows the build button as inactive while the stop button is active.

## Table of contents

### Enumeration Members

- [building](codearts_plugin_.BuildStatusType.md#building)
- [initial](codearts_plugin_.BuildStatusType.md#initial)
- [starting](codearts_plugin_.BuildStatusType.md#starting)
- [stopping](codearts_plugin_.BuildStatusType.md#stopping)

## Enumeration Members

### building

• **building** = ``2``

#### Defined in

[index.d.ts:16925](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16925)

___

### initial

• **initial** = ``0``

#### Defined in

[index.d.ts:16923](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16923)

___

### starting

• **starting** = ``1``

#### Defined in

[index.d.ts:16924](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16924)

___

### stopping

• **stopping** = ``3``

#### Defined in

[index.d.ts:16926](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16926)
