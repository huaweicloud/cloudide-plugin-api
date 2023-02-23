[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / Progress

# Interface: Progress<T\>

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).Progress

Defines a generalized way of reporting progress updates.

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Methods

- [report](cloudide_plugin_.Progress.md#report)

## Methods

### report

▸ **report**(`value`): `void`

Report a progress update.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `T` | A progress item, like a message and/or an report on how much work finished |

#### Returns

`void`

#### Defined in

[index.d.ts:5148](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5148)
