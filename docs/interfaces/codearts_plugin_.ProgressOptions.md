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

[index.d.ts:11312](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11312)

___

### location

• **location**: [`ProgressLocation`](../enums/codearts_plugin_.ProgressLocation.md) \| { `viewId`: `string`  }

The location at which progress should show.

#### Defined in

[index.d.ts:11298](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11298)

___

### title

• `Optional` **title**: `string`

A human-readable string which will be used to describe the
operation.

#### Defined in

[index.d.ts:11304](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11304)
