[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ProgressOptions

# Interface: ProgressOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).ProgressOptions

Value-object describing where and how progress should show.

## Table of contents

### Properties

- [cancellable](codearts_plugin_.ProgressOptions.md#cancellable)
- [location](codearts_plugin_.ProgressOptions.md#location)
- [title](codearts_plugin_.ProgressOptions.md#title)

## Properties

### cancellable

• `Optional` **cancellable**: `boolean`

Controls if a cancel button should show to allow the user to
cancel the long running operation.  Note that currently only
`ProgressLocation.Notification` is supporting to show a cancel
button.

#### Defined in

[index.d.ts:10988](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10988)

___

### location

• **location**: [`ProgressLocation`](../enums/codearts_plugin_.ProgressLocation.md) \| { `viewId`: `string`  }

The location at which progress should show.

#### Defined in

[index.d.ts:10974](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10974)

___

### title

• `Optional` **title**: `string`

A human-readable string which will be used to describe the
operation.

#### Defined in

[index.d.ts:10980](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L10980)
