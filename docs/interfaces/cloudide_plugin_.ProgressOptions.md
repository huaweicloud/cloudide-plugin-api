[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ProgressOptions

# Interface: ProgressOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ProgressOptions

Value-object describing where and how progress should show.

## Table of contents

### Properties

- [cancellable](cloudide_plugin_.ProgressOptions.md#cancellable)
- [location](cloudide_plugin_.ProgressOptions.md#location)
- [title](cloudide_plugin_.ProgressOptions.md#title)

## Properties

### cancellable

• `Optional` **cancellable**: `boolean`

Controls if a cancel button should show to allow the user to
cancel the long running operation.  Note that currently only
`ProgressLocation.Notification` is supporting to show a cancel
button.

#### Defined in

[index.d.ts:5118](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5118)

___

### location

• **location**: [`ProgressLocation`](../enums/cloudide_plugin_.ProgressLocation.md) \| { `viewId`: `string`  }

The location at which progress should show.

#### Defined in

[index.d.ts:5106](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5106)

___

### title

• `Optional` **title**: `string`

A human-readable string which will be used to describe the
operation.

#### Defined in

[index.d.ts:5111](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5111)
