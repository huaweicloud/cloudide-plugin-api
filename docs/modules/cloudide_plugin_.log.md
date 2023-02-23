[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](_cloudide_plugin_.md) / log

# Namespace: log

["@cloudide/plugin"](_cloudide_plugin_.md).log

User behavior record.

**`Param`**

Custom business scope.

**`Param`**

User behavior, eg. download, install, uninstalled.

**`Param`**

Behavioral data, eg. version, identifier, method, extension_name.

## Table of contents

### Functions

- [recordAction](cloudide_plugin_.log.md#recordaction)

## Functions

### recordAction

▸ **recordAction**(`scope`, `action`, `data?`): [`Thenable`](../interfaces/Thenable.md)<`string` \| `undefined`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `scope` | `string` |
| `action` | `string` |
| `data?` | `Object` |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`string` \| `undefined`\>

#### Defined in

[index.d.ts:11419](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L11419)
