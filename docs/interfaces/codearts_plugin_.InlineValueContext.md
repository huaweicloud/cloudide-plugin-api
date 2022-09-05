[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InlineValueContext

# Interface: InlineValueContext

["@codearts/plugin"](../modules/_codearts_plugin_.md).InlineValueContext

A value-object that contains contextual information when requesting inline values from a InlineValuesProvider.

## Table of contents

### Properties

- [frameId](codearts_plugin_.InlineValueContext.md#frameid)
- [stoppedLocation](codearts_plugin_.InlineValueContext.md#stoppedlocation)

## Properties

### frameId

• `Readonly` **frameId**: `number`

The stack frame (as a DAP Id) where the execution has stopped.

#### Defined in

[index.d.ts:3017](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L3017)

___

### stoppedLocation

• `Readonly` **stoppedLocation**: [`Range`](../classes/codearts_plugin_.Range.md)

The document range where execution has stopped.
Typically the end position of the range denotes the line where the inline values are shown.

#### Defined in

[index.d.ts:3023](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L3023)
