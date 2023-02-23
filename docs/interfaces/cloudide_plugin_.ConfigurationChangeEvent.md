[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ConfigurationChangeEvent

# Interface: ConfigurationChangeEvent

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ConfigurationChangeEvent

An event describing the change in Configuration

## Table of contents

### Methods

- [affectsConfiguration](cloudide_plugin_.ConfigurationChangeEvent.md#affectsconfiguration)

## Methods

### affectsConfiguration

▸ **affectsConfiguration**(`section`, `resource?`): `boolean`

Returns `true` if the given section for the given resource (if provided) is affected.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section` | `string` | Configuration name, supports _dotted_ names. |
| `resource?` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | A resource Uri. |

#### Returns

`boolean`

`true` if the given section for the given resource (if provided) is affected.

#### Defined in

[index.d.ts:5551](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5551)
