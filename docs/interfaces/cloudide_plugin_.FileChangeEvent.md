[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / FileChangeEvent

# Interface: FileChangeEvent

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).FileChangeEvent

The event filesystem providers must use to signal a file change.

## Table of contents

### Properties

- [type](cloudide_plugin_.FileChangeEvent.md#type)
- [uri](cloudide_plugin_.FileChangeEvent.md#uri)

## Properties

### type

• `Readonly` **type**: [`FileChangeType`](../enums/cloudide_plugin_.FileChangeType.md)

The type of change.

#### Defined in

[index.d.ts:5742](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5742)

___

### uri

• `Readonly` **uri**: [`Uri`](../classes/cloudide_plugin_.Uri.md)

The uri of the file that has changed.

#### Defined in

[index.d.ts:5747](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5747)
