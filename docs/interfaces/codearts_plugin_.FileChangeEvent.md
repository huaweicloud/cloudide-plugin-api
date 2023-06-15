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

[index.d.ts:7993](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L7993)

___

### uri

• `Readonly` **uri**: [`Uri`](../classes/codearts_plugin_.Uri.md)

The uri of the file that has changed.

#### Defined in

[index.d.ts:7998](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L7998)
