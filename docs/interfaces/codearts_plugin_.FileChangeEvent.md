[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / FileChangeEvent

# Interface: FileChangeEvent

["@codearts/plugin"](../modules/_codearts_plugin_.md).FileChangeEvent

The event filesystem providers must use to signal a file change.

## Table of contents

### Properties

- [type](codearts_plugin_.FileChangeEvent.md#type)
- [uri](codearts_plugin_.FileChangeEvent.md#uri)

## Properties

### type

• `Readonly` **type**: [`FileChangeType`](../enums/codearts_plugin_.FileChangeType.md)

The type of change.

#### Defined in

[index.d.ts:7933](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7933)

___

### uri

• `Readonly` **uri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The uri of the file that has changed.

#### Defined in

[index.d.ts:7938](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7938)
